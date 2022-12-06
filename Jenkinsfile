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

        stage('shell script testing') {
          steps {
            sh 'pwd'
          }
        }

        stage('a failed shell script') {
          steps {
            sh 'pad'
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