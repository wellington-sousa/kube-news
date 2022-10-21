pipeline {
    agent any

    stages {

        stage('Build Docker Image'){
            step {
                script {
                    dockerapp = docker.build("wellingtonsousa/kube-news:${env.BUILD_ID}", '-f ./src/Dockerfile ./src')
                }
            }
        }
    }}