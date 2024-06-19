pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }
        stage('Terraform Init') {
            steps {
                bat 'cd D:\\PROJECT\\Terraform\\"nginx test" && terraform init'
            }
        }
        stage('Terraform Apply') {
            steps {
                bat 'cd D:\\PROJECT\\Terraform\\"nginx test" && terraform apply -auto-approve'
            }
        }
    }
}
