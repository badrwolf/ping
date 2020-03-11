node {
  environment {
    FULL_PATH_BRANCH = "${sh(script:'git name-rev --name-only HEAD', returnStdout: true)}"
    GIT_BRANCH = FULL_PATH_BRANCH.substring(FULL_PATH_BRANCH.lastIndexOf('/') + 1, FULL_PATH_BRANCH.length())
  } 
  

  stage('Clone repo ') {
           
                checkout scm
            
  }

  stage('List pods') {
     sh 'printenv'
   }

  }

