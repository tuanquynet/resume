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
        sh '''
echo $USER'''
        sh 'npm install'
        sh 'apt-get update && apt-get install rsync -y'
        sh 'npm uninstall gitbook -g'
      }
    }
  }
  environment {
    HOME = '.'
  }
}