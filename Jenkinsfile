pipeline {
  environment {
    registry = "minthoang/alpine-tomcat-httpd-sshd"
    registryCredential = 'dockerhub'
  }
  agent any
  stages {
    stage('Building image') {
      steps{
        script {
          docker.build registry + ":$BUILD_NUMBER"
        }
      }
    }
  }
}
