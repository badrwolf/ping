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
                sh 'sudo  docker-compose stop pingfederate'
                sh 'sudo docker-compose rm -f pingfederate'
                sh 'sudo docker-compose up '
                
            }
        }
        stage('passed') {
            steps {
                echo 'docker-compose stop rm up with success hopeeeee'
            }
        }
    }
}
