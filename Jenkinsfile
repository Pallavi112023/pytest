pipeline {
  agent any
  stages {
    stage('get list of python package') {
      agent any
      steps {
        sh '''python3 -m pip -V
python3 -m pip freeze
'''
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