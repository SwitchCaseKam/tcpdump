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
        sh 'apk add gcc libc-dev openssl-dev make git libpcap-dev'
        sh './configure'
      }
    }
  }
}