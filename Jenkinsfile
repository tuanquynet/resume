pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'pwd'
        sh 'whoami'
        sh 'npm install gitbook -g'
        sh 'apt-get update && apt-get install rsync -y'
      }
    }
  }
}