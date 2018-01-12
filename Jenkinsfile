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
            bat(returnStatus: true, returnStdout: true, script: 'javac HelloWorld.java')
            bat(script: 'java HelloWorld', returnStatus: true, returnStdout: true)
            echo 'Run'
          }
        }
      }
    }
  }
}