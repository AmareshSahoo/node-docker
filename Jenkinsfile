pipeline {
  agent any
  stages {
    stage('Install Dependancy') {
      steps {
        sh '''echo "Install Dependancies"
npm install'''
        sh 'echo "Done"'
      }
    }

    stage('Build') {
      steps {
        sh '''echo "Build Started"
docker version
docker build .'''
      }
    }

  }
}