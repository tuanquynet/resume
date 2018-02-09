pipeline {
  agent {
    docker {
      image 'node:8.9.1'
      args '-p 3000:3000'
    }
    
  }
  stages {
    stage('Build') {
      steps {
        sh 'pwd'
        sh 'npm install gitbook-cli'
        sh 'sudo apt-get update && sudo apt-get install rsync -y'
      }
    }
  }
  environment {
    HOME = '.'
  }
}