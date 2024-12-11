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
      container('mavencontainer') {  
          sh "echo 'it's working'"
       }    
      }
    }
  }
}
