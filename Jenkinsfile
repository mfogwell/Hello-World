pipeline {
  agent any
  stages {
    stage('error') {
      steps {
        fileExists 'notthere.html'
      }
    }
  }
}