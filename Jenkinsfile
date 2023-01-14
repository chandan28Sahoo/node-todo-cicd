pipeline {
  agent any
  stages {
    stage('checkout_code') {
      steps {
        git(url: ' https://github.com/chandan28Sahoo/node-todo-cicd', branch: 'master')
      }
    }

    stage('logs') {
      steps {
        sh 'ls -la'
      }
    }

  }
}