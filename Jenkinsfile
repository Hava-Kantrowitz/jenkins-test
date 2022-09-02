pipeline {
  agent any
  stages {
    stage('version') {
      steps {
        sh 'python3 --version'
      }
    }
    stage('hello') {
      steps {
        sh 'python3 tester.py'
      }
    }
  }
  post {
    success {
      echo 'This jenkins pipeline was successful'
    }
    failure {
      echo 'This jenkins pipeline failed'
    }
  }
}
