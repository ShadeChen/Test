pipeline {
  agent any
  stages {
    stage('Checkout Code') {
      steps {
        git(url: 'https://github.com/ShadeChen/Test.git', branch: 'dev')
      }
    }

    stage('Front-end Test') {
      steps {
        powershell 'npm run test:unit'
      }
    }

  }
}