pipeline {
  agent any
  stages {
    stage('CheckOut Code') {
      steps {
        git(url: 'https://github.com/T0KaG/jenkins_test', branch: 'main')
      }
    }

    stage('log') {
      steps {
        sh 'ls -laht'
      }
    }

    stage('Build') {
      steps {
        sh 'docker build -f jenkins_test/Dockerfile .'
      }
    }

  }
}