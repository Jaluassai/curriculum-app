pipeline {
  agent {
    docker {
      image 'node:lts-alpine'
    }

  }
  stages {
    stage('checkout') {
      steps {
        git(url: 'https://github.com/Jaluassai/curriculum-app', branch: 'dev')
      }
    }

    stage('dsad') {
      steps {
        sh 'ls -la'
      }
    }

  }
}