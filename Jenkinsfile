pipeline {
  agent any
  stages {
    stage('') {
      steps {
        withMaven(jdk: 'jdk11', maven: 'maven3') {
          sh 'nvm compile'
        }

      }
    }

  }
  environment {
    AUTHOR = 'Luke'
  }
}