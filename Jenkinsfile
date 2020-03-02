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
                sh ' kubectl scale deployment pingfederate  --replicas=0 -n default'
                
            }
        }
        stage('passed') {
            steps {
                echo 'docker-compose stop rm up with success hopeeeee'
            }
        }
    }
}
