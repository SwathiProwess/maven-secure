pipeline {
  agent any
  environment {
    CLIENT_ID = credentials('connectedAppClientId')
  }
  stages {
    stage('Build') {
      steps {
        sh 'mvn clean install -Dclient.id=$CLIENT_ID'
      }
    }
  }
}
