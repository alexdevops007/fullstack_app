pipeline {
  agent any
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
        sh 'curl -s https://deb.nodesource.com/setup_16.x | bash && apt install nodejs -y'
      }
    }

  }
}