[2;2R{ 
  

  stage('Clone repo ') {
           
                checkout scm
            
  }

 stage('List pods') {
    withKubeConfig([credentialsId: 'user1',
                    serverUrl: 'https://192.168.0.199/',
                    clusterName: 'testlab',
                    namespace: 'default'
                    ]) {
      sh 'kubectl get deployments -n default --insecure-skip-tls-verify '
    }
  }

  }

