pipeline {
    agent any
    stages {
        stage('scm') {
            steps {
                git credentialsId: 'github-credentials', url: 'https://github.com/itsmaheshbabu/ntier-terraform.git'
            }
        }
        stage('init') {
            steps {
                sh 'terraform init'
            }
        }
        stage('validate') {
            steps {
                sh 'terraform validate'
            }
        }
        stage('apply') {
            steps {
                sh 'terraform apply -var-file="values.tfvars" --auto-approve'
            }
        }
        stage('destroy') {
              steps {
                  sh 'terraform destroy --auto-approve'
             }
       }
    }
}

