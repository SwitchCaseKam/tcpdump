pipeline {
  agent any
  stages {
    stage('Build') {
      agent {
        docker {
          image 'ubuntu'
        }

      }
      steps {
        sh 'sudo apt install gcc'
        sh './configure'
      }
    }
  }
}