pipeline {
    agent any
  

    stages {
        stage('checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/SirishaReddy1234/ec2_using_jenkins.git'
            }

        }
        stage('terraform init') {
            steps {
                
                sh 'terraform init'
              
            }
        
       }
       stage('terraform plan') {
            steps {
                
                sh 'terraform plan'
              
            }
        
       }
       stage('terraform apply') {
            steps {
                
                sh 'terraform apply -auto-approve'
              
            }
        
       }
       
       
    }
}
