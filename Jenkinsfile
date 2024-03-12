pipeline {
    agent any
    
    stages {
        stage('Clone Repository') {
            steps {
                // Checkout your code from the Git repository
                git branch: 'main', url: 'https://github.com/ravitejajyosula/bw-assign.git'
            }
        }
        stage('Build Docker Image') {
            steps {
                script {
                    dockerImage = docker.build('nodejs_custom:latest', '-f docker/Dockerfile .')
                }
            }
        }
        
        }
    }
