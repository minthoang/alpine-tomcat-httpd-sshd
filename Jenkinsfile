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
  stage('Test') {
            steps {
                sh 'docker images'
                sh 'docker ps -a'
            }
        }
  }
  environment {
    registry = 'minthoang/alpine-tomcat-httpd-sshd'
    registryCredential = 'dockerhub'
  }
}
