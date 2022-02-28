pipeline {
  agent any
  stages {
    stage('docker') {
      steps {
        sh 'docker build -t new-image .'
        sh 'docker run -p "3000:3000" my-image'
      }
    }

  }
}