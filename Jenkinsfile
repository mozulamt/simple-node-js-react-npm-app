pipeline {
    agent {
        docker {
            image ('node:6-alpine')
            customWorkspace {
                withEnv([
                    'npm_config_cache=npm-cache',
                    'HOME=.',
                ])
            } 
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
