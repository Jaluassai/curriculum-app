pipeline {
  agent any
  stages {
    stage('checkout') {
      steps {
        git(url: 'https://github.com/Jaluassai/curriculum-app', branch: 'dev')
      }
    }

    stage('dsad') {
      parallel {
        stage('dsad') {
          steps {
            sh 'ls -la'
          }
        }

        stage('FrontTest') {
          steps {
            sh 'cd curriculum-front && npm i && npm run test:unit'
          }
        }

      }
    }

  }
}