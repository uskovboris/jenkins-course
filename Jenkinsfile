pipeline {
  agent: any

  stages {

    stage('Check Agent') {
      agent any
      steps {
        echo 'Running on agent...'
        sh 'hostname'
        echo "Path to workspace '{WORKSPACE}'"
        echo "Node name '{NODE_NAME}'"
      }
    }

    stage('Build Info') {
      agent any
      steps {
        echo 'Build information..."'
        echo "Build number '{BUILD_NUMBER}'"
        echo "Build ID '{BUILD_ID}'"
        echo "Build URL '{BUILD_URL}'"
      }
    }
    
  }
}
