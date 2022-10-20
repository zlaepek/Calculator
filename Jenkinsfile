pipeline {
  agent any
  stages {
    stage('chmod') {
      steps {
        sh '''chmod 777 gradlew
ls -l gradlew'''
      }
    }

    stage('Unit test') {
      steps {
        sh './gradlew test'
      }
    }

  }
}