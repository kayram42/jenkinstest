pipeline {
  agent {
    kubernetes {
      yamlFile 'agent.yaml'
      idleMinutes 1
    }
  }
  stages {
    stage('Build maven code') {
      steps {
      container('dockercontainer') {  
          sh "echo 'it's working'"
       }    
      }
    }
  }
}
