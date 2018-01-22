pipeline {
    agent {
        docker {
            image 'node:6-alpine'
            args '-v $HOME/.npm:/root/.npm'
            args '-p 3000:3000'
        }
    }
    stages {
        stage('Build') {
            steps { 
                sh 'npm install' 
            }
        }
    }
}
