pipeline {
  agent {
    docker {
      image 'node:16-alpine'
    }

  }
  stages {
    stage('Checkout Code') {
      steps {
        git(url: 'https://github.com/alexdevops007/fullstack_app', branch: 'dev')
      }
    }

    stage('Log') {
      steps {
        sh 'ls -la'
      }
    }

    stage('Install npm') {
      steps {
        sh 'npm install'
      }
    }

  }
}