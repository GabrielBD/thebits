pipeline {
  agent any
  stages {
    stage('Test') {
      steps {
        echo 'Build'
        echo 'Hola'
      }
    }
    stage('Deploy') {
      parallel {
        stage('Deploy') {
          steps {
            echo 'Deploy'
            sh 'maven clean'
          }
        }
        stage('Notify') {
          steps {
            echo 'Notificacion'
          }
        }
      }
    }
  }
}