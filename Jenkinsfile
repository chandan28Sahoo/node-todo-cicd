pipeline {
  agent any
  stages {
    stage('checkout_code') {
      steps {
        git(url: ' https://github.com/chandan28Sahoo/node-todo-cicd', branch: 'master')
      }
    }

    stage('logs') {
      parallel {
        stage('logs') {
          steps {
            sh 'ls -la'
          }
        }

        stage('back-end-run') {
          steps {
            sh 'docker-compose up -d'
          }
        }

      }
    }

  }
}