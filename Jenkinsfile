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
            sh 'chmod 777 gradlew'
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