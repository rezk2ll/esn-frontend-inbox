pipeline {

  agent { 
    dockerfile {
      filename 'Dockerfile'
      dir 'test'
    }
  }

  stages {
    stage('Install packages') {
      steps {
        sh 'npm install'
      }
    }

    stage('Run tests') {
      steps {
        sh 'npm run test'
      }
    }
  }
}
