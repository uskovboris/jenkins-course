pipeline {
  agent none

  stages {

    stage('Check Agent') {
      agent any
      steps {
        echo 'Running on agent...'
        sh 'hostname'
        echo "Path to workspace '${WORKSPACE}'"
        echo "Node name '${NODE_NAME}'"
      }
    }

    stage('Build Info') {
      agent any
      steps {
        echo 'Build information..."'
        echo "Build number '${BUILD_NUMBER}'"
        echo "Build ID '${BUILD_ID}'"
        echo "Build URL '${BUILD_URL}'"
      }
    }

    stage('System Details') {
      agent any
      steps {
        echo "OS:"
        sh "uname -a"
        echo "User:"
        sh "whoami"
        echo "Current directory:"
        sh "pwd"
        echo "Workspace files:"
        sh "ls -la '${WORKSPACE}'"
        def status = sh(script:"free -h", returnStatus:true)
        if (status != 0) {
          echo "Memory check skipped"
        }
        echo "Dete and time"
        sh "date"
      }
    
  }
}
