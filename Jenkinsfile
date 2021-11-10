pipeline {
    agent any
    stages {
        stage('scm') {
            steps {
                git credentialsId: 'github-credentials', url: 'https://github.com/itsmaheshbabu/ntier-terraform.git'
            }
        }
        stage('init) {
              steps {
                  sh 'terraform init'
    }
}

