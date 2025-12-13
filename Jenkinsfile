pipeline {
  agent: any

  stages {
    stage('Check Agent') {
      steps {
        echo 'Running on agent...'
        sh 'hostname'
        echo "Path to workspace '{WORKSPACE}'"
        echo "Node name '{NODE_NAME}'"
      }
    }
    
  }
}
