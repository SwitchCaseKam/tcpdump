pipeline {
  agent any
  stages {
    stage('Build') {
      agent {
        docker {
          image 'alpine'
        }

      }
      steps {
        sh './configure'
        sh 'sudo apt install gcc'
      }
    }
  }
}