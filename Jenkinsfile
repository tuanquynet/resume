pipeline {
  agent {
    docker {
      image 'node:8.9.1'
      args '-p 3000:3000 -u root:sudo -v $HOME/.npm:/root/.npm'
    }
    
  }
  stages {
    stage('Build') {
      steps {
        sh 'pwd'
        sh 'npm install gitbook-cli -g'
        sh 'apt-get update'
        sh 'apt-get install rsync -y'
        sh 'npm install'
        sh 'npm run build'
        sh 'ls _book'
      }
    }
  }
  environment {
    HOME = '.'
  }
}