node {
  environment {
    FULL_PATH_BRANCH = "${sh(script:'git name-rev --name-only HEAD', returnStdout: true)}"
    GIT_BRANCH = FULL_PATH_BRANCH.substring(FULL_PATH_BRANCH.lastIndexOf('/') + 1, FULL_PATH_BRANCH.length())
  } 
  

  stage('Clone repo ') {
           
                checkout scm
            
  }

  stage('List pods') {
    withKubeConfig([credentialsId: 'user1',
                   
                    serverUrl: 'https://192.168.0.199',
                  
                    clusterName: 'testlab',
                    namespace: 'default'
                    ]) {
            echo 'Pulling... ' + env.GIT_BRANCH

    }
  }
}
