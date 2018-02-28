pipeline {
  agent any
  stages {
    stage('Checkout') {
      steps {
        fileExists 'notthere.html'
        checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[credentialsId: 'github', url: 'https://github.com/mfogwell/Hello-World.git']]])
      }
    }
  }
}