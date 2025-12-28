pipeline {
  agent any

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
          echo "Replace result: {message.replace('Tutorial', 'Course')}"
        }
      }
    }
    
  } // stages

} // pipeline
