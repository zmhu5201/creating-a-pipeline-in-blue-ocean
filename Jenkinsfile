pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        sh '''npm install
'''
      }
    }

    stage('Test') {
      steps {
        sh './jenkins/scripts/test.sh'
      }
    }

  }
}