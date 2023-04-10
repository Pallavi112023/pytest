pipeline {
  agent any
  stages {
    stage('checkout') {
      agent any
      steps {
        git(url: 'https://github.com/faraday-academy/curriculum-app', branch: 'dev')
      }
    }

  }
}