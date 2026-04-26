pipeline {
    agent any

    stages {
        stage('Build Docker Image') {
            steps {
                sh 'docker build -t ci-app .'
            }
        }

        stage('Run Container') {
            steps {
                sh 'docker run ci-app'
            }
        }
    }
}