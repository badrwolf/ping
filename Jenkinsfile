pipeline {
    agent any

    stages {
        stage('Clone repo ') {
            steps{
                checkout scm
            }
        }
        stage('Test') {
            steps {
                sh ' cd /root/ping '
                sh 'docker-compose down'
                sh 'docker-compose up'
            }
        }
        stage('passed') {
            steps {
                echo 'waaaayli dazeeet'
            }
        }
    }
}
