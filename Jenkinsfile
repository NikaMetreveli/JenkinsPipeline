pipeline {
  agent any
  stages {
    stage('version check') {
      parallel {
        stage('version check') {
          steps {
            bat 'cmd mvn --version'
          }
        }

        stage('run program') {
          steps {
            bat 'cmd mvn clean test'
          }
        }

      }
    }
  tools {
    maven 'Maven3'
  }
    
}