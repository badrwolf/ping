 node {
  stage('poll scm') {
      checkout scm
  }
 

  stage('Apply Kubernetes files') {
    withKubeConfig([credentialsId: 'user1', serverUrl: 'https://192.168.0.199']) {
      sh 'kubectl scale deployment pingfederate  --replicas=0 -n default'
    }
  }
}
