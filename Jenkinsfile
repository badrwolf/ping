node { 
  

  stage('Clone repo ') {
           
                checkout scm
            
  }

 stage('List pods') {
    withKubeConfig([credentialsId: 'user1',
                    serverUrl: 'https://192.168.0.199/v3',
                    clusterName: 'testlab',
                    namespace: 'default'
                    ]) {
      sh 'kubectl get pods -n default '
    }
  }

  }

