pipeline {
    agent any
    tools {
        dockerTool 'MYDOCKER'
    }

    stages {
        stage('Version') {
            steps {
                sh 'docker --version'
            }
        }
     
        stage('Build') {
            steps {
                sh 'docker build -t kodekloud:v1 .'
            }
        }
    }
}

