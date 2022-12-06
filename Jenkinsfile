pipeline {
  agent any
  stages {
    stage('Check out code') {
      parallel {
        stage('Check out code') {
          steps {
            git(url: 'https://github.com/tungduonghgg123/curriculum-app', branch: 'dev')
          }
        }

        stage('Say some thing cool') {
          steps {
            echo 'ahihi'
          }
        }

      }
    }

    stage('Print Hello World') {
      steps {
        echo 'Hello World'
      }
    }

  }
}