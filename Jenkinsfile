pipeline {
  agent any
  stages {
    stage('Compile') {
      steps {
        sh 'mvn compile'
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