pipeline {
    agent { dockerfile true }
    stages {
        stage('Test') {
            steps {
                sh "docker logs ${c.id}"
         
            }
        }
    }
}
