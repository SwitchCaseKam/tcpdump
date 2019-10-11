pipeline {
  agent any
  stages {
    stage('Build') {
      agent {
        docker {
          image 'alpine'
          args '-u 0'
        }

      }
      steps {
        sh 'env'
        sh 'apk add gcc libc-dev openssl-dev make git libpcap-dev'
        sh './configure'
        sh 'make'
      }
    }
  }
}