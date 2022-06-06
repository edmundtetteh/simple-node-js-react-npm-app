pipeline {
    agent {
        docker {
            image 'node:lts-bullseye-slim' 
            args '-p 3000:3000' 
        }
    }
    tools {
        nodejs "node"
    }
    stages {
        stage('Build') {
            environment {
                  HOME="."
                }
            steps {
                sh 'npm install' 
            }
        }
    }
}
