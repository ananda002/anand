pipeline {
  agent any
  stages {
    stage('build') {
      parallel {
        stage('build') {
          steps {
            sh 'echo "hi"'
          }
        }
        stage('trigger') {
          steps {
            sh 'echo "dgg"'
          }
        }
      }
    }
    stage('depoly') {
      steps {
        sh 'echo "hello"'
      }
    }
    stage('test') {
      steps {
        sh 'echo "tst"'
      }
    }
  }
}