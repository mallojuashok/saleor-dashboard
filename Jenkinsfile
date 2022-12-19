pipeline {
    agent any
    triggers {
        pollSCM('* * * * *')
    }
    stages {
        stage('GIT') {
            steps {
                git branch: 'main', url: 'https://github.com/mallojuashok/saleor-dashboard.git'
            }
        }
        stage('docker image build') {
            steps {
                sh 'docker image build -t ashokachary/saleor-dashboard:DEV .'
            }
        }
        
    }
}