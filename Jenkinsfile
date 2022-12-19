pipeline{
    agent any
    triggers {
        pollSCM('* * * * *')
    }
    stages {
        stage{
            steps('GIT'){
                git branch:'main', url:'https://github.com/mallojuashok/saleor-dashboard.git'
            }
        }
        stage{
            steps('DOCKER IMAGE BUILD'){
                sh 'docker image build -t ashokachary/saleor:DEV .'
            }
        }
        
    }
}