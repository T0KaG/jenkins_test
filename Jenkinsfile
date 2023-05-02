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

  }
}