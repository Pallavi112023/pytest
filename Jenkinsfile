pipeline {
  agent any
  stages {
    stage('checkout') {
      agent any
      steps {
        git 'https://github.com/Pallavi112023/circuit'
      }
    }

    stage('get files') {
      steps {
        sh 'ls -la'
      }
    }

  }
}