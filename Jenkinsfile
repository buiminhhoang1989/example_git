pipeline {
  agent any
  stages {
    stage('Build') {
      parallel {
        stage('Build') {
          steps {
            echo 'Build start'
          }
        }
        stage('Run ') {
          steps {
            sh '''javac HelloWorld.java
java HelloWorld'''
          }
        }
      }
    }
  }
}