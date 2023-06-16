pipeline {
    agent any
    tools {
        dockerTool 'mydocker'
    }

    stages {
        stage('Version') {
            steps {
                sh 'docker --version'
            }
        }
        stage('Start Docker') {
            steps {
                sh 'sudo dockerd'
            }
        }
        stage('Build') {
            steps {
                sh 'docker build -t kodekloud:v1 .'
            }
        }
    }
}

