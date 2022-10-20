pipeline {
  agent any
  stages {
    stage('compile') {
      steps {
        sh 'sudo ./gradlew compileJava'
      }
    }

    stage('Unit test') {
      steps {
        sh 'sudo ./gradlew test'
      }
    }

  }
}