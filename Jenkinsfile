pipeline {
  agent any
  stages {
    stage('Install Dependancy') {
      steps {
        sh '''Echo "Install Dependancies"
npm install'''
        sh 'Echo "Done"'
      }
    }

    stage('Build') {
      agent {
        node {
          label 'node'
        }

      }
      steps {
        sh '''docker version
docker build .'''
      }
    }

  }
}