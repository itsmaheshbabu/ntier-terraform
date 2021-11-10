pipeline {
    agent any
    stages {
        stage('scm') {
            steps {
                git branch: 'master', url: 'https://github.com/itsmaheshbabu/ntier-terraform.git'
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
    }
}