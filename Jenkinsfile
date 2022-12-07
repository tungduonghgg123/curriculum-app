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

        stage('echo PATH') {
          steps {
            sh 'echo "PATH is: $PATH"'
          }
        }

      }
    }

    stage('Run unit test') {
      steps {
        sh 'cd curriculum-front && /usr/local/bin/npm i && npm run test:unit'
      }
    }

  }
}