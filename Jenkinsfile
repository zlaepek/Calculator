pipeline {
  agent any
  stages {
    stage('compile') {
      parallel {
        stage('compile') {
          steps {
            sh './gradlew compileJava'
          }
        }

        stage('test') {
          steps {
            sh './gradlew test'
          }
        }

        stage('error') {
          steps {
            sh 'ls -l gradlew'
          }
        }

      }
    }

    stage('Unit test') {
      steps {
        sh './gradlew test'
      }
    }

  }
}