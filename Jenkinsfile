pipeline {
  agent any
  tools{
    maven 'maven_3_9_1'
  }
  stages {
    stage('Buils Maven'){
      steps{
         sh 'mvm clean install'
      }  
    }
    stage('CheckOut Code') {
      steps {
        git(url: 'https://github.com/T0KaG/jenkins_test', branch: 'main')
      }
    }

    stage('log') {
    
    }

  }
}
