 node {
  stage('poll scm') {
      checkout scm
  }
 

  stage('Apply Kubernetes files') {
    withKubeConfig() {
      sh 'kubectl scale deployment pingfederate  --replicas=0 -n default'
    }
  }
}
