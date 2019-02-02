pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        echo 'Building....'
      }
    }
    stage('Test Firefox') {
      parallel {
        stage('Test Firefox') {
          steps {
            sh 'echo \'Testing Firefox\''
          }
        }
        stage('Test Chrome') {
          steps {
            sh 'echo \'Test chrome\''
          }
        }
      }
    }
    stage('Deploy') {
      steps {
        echo 'Deploy'
      }
    }
  }
}