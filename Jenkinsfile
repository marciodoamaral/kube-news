pipeline {
    agent any

    stages {
        stage('Build Docker Image') {
            steps {
                script {
                    dockerapp = docker.build("fabricioveronez/kube-news:latest", '-f ./src/Dockerfile ./src')
                }
            }
        }
    }
} 