
 def getGitBranchName() {
    return scm.branches[0].name
}

node { 
  

  stage('Clone repo ') {
           
                checkout scm
            
  }

  stage('List pods') {
     sh 'printenv'
   }

  }

