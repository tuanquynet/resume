pipeline {
  agent {
    docker {
      image 'node:8.9.1'
    }
    
  }
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