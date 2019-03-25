pipeline {
  agent any
  stages {
    stage('checkout') {
      steps {
        sh 'echo 1'
        sh 'echo 2'
      }
    }
    stage('build01') {
      parallel {
        stage('build01') {
          steps {
            sh 'echo build0101'
            sh 'echo build0102'
          }
        }
        stage('build02') {
          steps {
            sh 'echo build0201'
            sh 'echo build0202'
          }
        }
      }
    }
    stage('deploy') {
      steps {
        sh 'echo deploy'
      }
    }
  }
}