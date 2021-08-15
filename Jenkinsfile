pipeline {
  agent any
  stages {
    stage('error') {
      steps {
        withMaven(jdk: 'jdk11', maven: 'maven3') {
          sh 'mvn compile'
        }

      }
    }

  }
  environment {
    AUTHOR = 'Luke'
  }
}