pipeline {
  agent any
  stages {
    stage('Building image') {
      steps {
        script {
          docker.build registry + ":$BUILD_NUMBER"
        }

      }
    }

  }
  environment {
    registry = 'minthoang/alpine-tomcat-httpd-sshd'
    registryCredential = 'dockerhub'
  }
}