pipeline {
  agent {
    // this image provides everything needed to run Cypress
    any {
      image 'cypress/base:10'
    }
  }

  stages {
    stage('build and test') {
      steps {
        sh 'npm ci'
        sh "npm run test:ci"
      }
    }
  }
}