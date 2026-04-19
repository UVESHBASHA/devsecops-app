pipeline {
  agent any

  stages {

    stage('Build Docker Image') {
      steps {
        sh 'docker build -t devsecops-app .'
      }
    }

    stage('Run Container') {
      steps {
        sh 'docker run -d -p 80:3000 devsecops-app'
      }
    }

  }
}
