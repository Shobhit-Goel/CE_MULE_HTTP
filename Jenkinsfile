pipeline {
  agent any
  stages {
    stage('Deploy CloudHub') {
      environment {
        ANYPOINT_CREDENTIALS = credentials('CloudhubID')
      }
      steps {
        sh 'mvn deploy  -Duser=${ANYPOINT_CREDENTIALS_USR} -Dpassword=${ANYPOINT_CREDENTIALS_PSW}'
      }
    }
  }
}
