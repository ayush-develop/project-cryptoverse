pipeline {
  agent any

  stages {
    stage('Build') {
      steps {
        // Install dependencies
        sh 'npm install'

        // Build React app
        sh 'npm run build'
      }
    }

    stage('Test') {
      steps {
        // Run tests
        sh 'npm run test'
      }
    }

    stage('Deploy') {
      steps {
        // Deploy to production server
        sh 'npm run deploy'
      }
    }
  }
}
