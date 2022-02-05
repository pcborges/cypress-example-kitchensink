pipeline {
  agent {
    // this image provides everything needed to run Cypress
    any {
      image 'cypress/base:10'
    }
  }

  tools {
    nodejs "nodejs"
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