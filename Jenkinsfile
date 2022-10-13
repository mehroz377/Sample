pipeline {
  agent any
    
  tools {nodejs "node"}
    
  stages {
     
    stage('Build') {
      steps {
        sh 'npm install'
      }
    }  
  }
  post {
    failure {
      echo 'Processing failed'
    }
    success {
      echo 'Processing succeeded'
    }
  }
}
