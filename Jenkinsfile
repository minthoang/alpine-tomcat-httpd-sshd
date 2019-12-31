pipeline {
  agent {
    dockerfile {
      filename 'Dockerfile'
    }

  }
  stages {
    stage('Test') {
      steps {
        sh 'docker build https://github.com/minthoang/alpine-tomcat-httpd-sshd.git'
      }
    }

  }
}