pipeline {
    agent any
    stages {
        stage('Gitcheckout') {
            steps {
                git branch: 'master', url: 'https://github.com/itsmaheshbabu/ntier-terraform.git'
            }
        }
    }
}