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
                sh ' cd /var/lib/jenkins/ '
                sh 'sudo  docker-compose up'
                
            }
        }
        stage('passed') {
            steps {
                echo 'waaaayli dazeeet'
            }
        }
    }
}
