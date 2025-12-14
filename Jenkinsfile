pipeline {
  agent: any

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
  }
  
}
