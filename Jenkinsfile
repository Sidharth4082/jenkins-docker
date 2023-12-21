pipeline {
    agent any
    stages {
        stage('Version') {
            steps {
                bat 'docker --version'
            }
        }
     
        stage('Build') {
            steps {
                bat 'docker build -t kodekloud:v1 .'
            }
        }
    }
}

