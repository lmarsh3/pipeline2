pipeline {
  agent any
  stages {
    stage('Compile') {
      steps {
        withMaven(jdk: 'jdk11', maven: 'maven3') {
          sh 'mvn compile'
        }

      }
    }

    stage('Unit Testing') {
      steps {
        withMaven(jdk: 'jdk11', maven: 'maven3') {
          sh 'mvn test'
        }

      }
    }

    stage('Publish Test Result') {
      steps {
        withMaven(jdk: 'jdk11', maven: 'maven3') {
          junit 'target/**/*.xml'
        }

      }
    }
  }
  environment {
    AUTHOR = 'Luke'
  }
}
