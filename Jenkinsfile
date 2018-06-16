pipeline {
  agent none
  stages {
    stage('Github Checkout') {
      steps {
        echo 'Revisando modificaciones en el repositorio'
      }
    }
    stage('Run Automatics Tests') {
      steps {
        echo 'Corriendo los tests con maven'
      }
      tools {
        maven 'maven'
      }
    }
    stage('Deploy to Stagging') {
      steps {
        echo 'Enviar al entorno de Producción para Test Humanos'
      }
    }
    stage('Slacks') {
      steps {
        echo 'Notificaciones al canal de Slack del equipo'
      }
    }
  }
}