pipeline {
    agent any

    stages {
        stage('Clone') { // Corrected stage name capitalization
            steps {
                git branch: 'main', url: 'https://github.com/Damu9393/Maven_project.git'
            }
        }
        stage('Init') { // Corrected stage name capitalization
            steps {
                sh 'terraform init'
            }
        }
        stage('Plan') { // Corrected stage name capitalization
            steps {
                sh 'terraform plan'
            }
        }
        stage('Apply') { // Changed second 'plan' to 'Apply'
            steps {
                sh 'terraform apply -auto-approve'
            }
        }
    }
}
