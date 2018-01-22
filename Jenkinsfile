pipeline {
    agent {
        docker {
            image 'node:6-alpine'
            args 'npm_config_cache=npm-cache'
            args 'HOME=.'
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
