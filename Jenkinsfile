pipeline {
  agent any
  stages {
    stage('CheckOut Code') {
      steps {
        git(url: 'https://github.com/T0KaG/jenkins_test', branch: 'main')
      }
    }

    stage('log') {
      parallel {
        stage('log') {
          steps {
            sh 'ls -laht'
          }
        }

        stage('log_1') {
          steps {
            sh 'pwd'
          }
        }

      }
    }

  }
}