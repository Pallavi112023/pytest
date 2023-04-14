pipeline {
  agent any
  stages {
    stage('checkout') {
      agent any
      steps {
        git(url: 'https://github.com/faraday-academy/curriculum-app', branch: 'dev')
      }
    }

    stage('get files') {
      steps {
        sh 'ls -la'
      }
    }

    stage('get python version') {
      steps {
        sh 'python3 -V'
      }
    }

  }
}