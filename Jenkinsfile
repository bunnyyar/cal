pipeline {
    agent any
    
    tools {
        nodejs 'nodejs'
    }

    stages {
        stage('Checkout') {
            steps {
                git git branch: 'main', credentialsId: '1ea4a13c-dba8-46f3-8c68-ecf3f9371f57', url: 'https://github.com/bunnyyar/cal'
            }
        }
        
        stage('Build') {
            steps {
                sh 'npm install'
                sh 'npm run build'
            }
        }
    }
    
}
