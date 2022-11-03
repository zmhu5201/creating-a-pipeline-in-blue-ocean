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
      agent {
        node {
          label 'CI'
        }

      }
      environment {
        CI = 'true'
      }
      steps {
        sh './jenkins/scripts/test.sh'
      }
    }

  }
}