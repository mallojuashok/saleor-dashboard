pipeline{
    agent any
    stages{
        stage{
            step('GIT'){
                git branch: 'main' , url: 'https://github.com/mallojuashok/saleor-dashboard.git'
            }
        }
        stage{
            step('DOCKER IMAGE BUILD'){
                sh 'docker image build -t ashokachary/saleor:DEV .'
            }
        }
        
    }
}