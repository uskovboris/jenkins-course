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

    stage('System Details') {
      agent any
      steps {
        sh '''#!/bin/bash
              echo 'Build information..."
              echo "OS '$(uname -a)'"
              echo "User '$(whoami)'"
              echo "Current directory '$(pwd)'"
              echo "Workspace files:"
              sh 'ls -la'
              
         '''
      }
    }
    
  }
}
