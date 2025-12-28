pipeline {
  agent any

  environment {
    BUILD_NUMBER = 2а
    APP_VERSION = '0.0.0'
  } // environment

  stages {

    stage('Variables Demo') {
      steps {
        script {
          def appName = "MyApplication"
          def port = 8080
          def isProduction = false

          echo "Application name: ${appName}"
          echo "Port: ${port}"
          echo "Is production build: ${isProduction}"
        }
      }
    }

    stage('String Operations') {
      steps {
        script {
          def message = 'Jenkins Pipeline Tutorial'
          echo "Upper case: ${message.toUpperCase()}"
          echo "Lower case: ${message.toLowerCase()}"
          echo "Replace result: ${message.replace('Tutorial', 'Course')}"
        }
      }
    }

    stage('Build Version') {
      steps {
        script {
          def major = '1'
          def minor = '0'
          env.APP_VERSION = "${major}.${minor}.${BUILD_NUMBER}"
          echo "Application version: [${env.APP_VERSION}]"
        }
      }
    }
    
  } // stages

} // pipeline
