pipeline {
    agent any

    stages {
        stage('Build Docker Image') {
            steps {
                script {
                    // Build Docker image for Django app
                    docker.build("my_django_app", ".")
                }
            }
        }
        
        stage('Deploy Docker Compose') {
            steps {
                script {
                    // Deploy Docker Compose stack
                    sh "docker-compose up -d"
                }
            }
        }
    }

