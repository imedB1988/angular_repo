pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        sh 'npm install'
      }
    }

    stage('test ') {
      steps {
        sh 'npm test'
      }
    }

    stage('log') {
      steps {
        sh 'ls -al'
      }
    }

    stage('checkout') {
      steps {
        git(url: 'https://github.com/imedB1988/angular_repo.git', branch: 'master')
      }
    }

  }
}