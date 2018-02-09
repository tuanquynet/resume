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
        sh '''
echo $USER'''
        sh 'npm install gitbook-cli -g'
        sh 'apt-get update && apt-get install rsync -y'
        sh 'npm uninstall gitbook -g'
      }
    }
  }
}