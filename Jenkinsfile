pipeline {
  agent any
  stages {
    stage('version check') {
      parallel {
        stage('version check') {
          steps {
            bat 'mvn --version'
          }
        }

        stage('run program') {
          steps {
            bat 'mvn clean test'
          }
        }

      }
    }

  }
}