pipeline {
  agent any
  stages {
    stage('install django') {
      steps {
        sh 'python3 -m pip install django'
      }
    }

    stage('check django') {
      steps {
        sh 'python3 -m django --version'
      }
    }

    stage('create new site') {
      steps {
        sh 'django-admin startproject mysite'
      }
    }

    stage('django run test') {
      steps {
        sh '''cd mysite
python manage.py runserver 172.105.62.142:8090'''
      }
    }

  }
}