pipeline {
  agent any
  stages {
    stage('compile') {
      steps {
        sh 'sh "./gradlew compileJava"'
      }
    }

    stage('Unit test') {
      steps {
        sh 'sh "./gradlew test"'
      }
    }

  }
}