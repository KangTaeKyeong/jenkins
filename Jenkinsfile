pipeline {
  agent any
  stages {
    stage('buile') {
      steps {
        sh 'sudo yum install -y httpd'
      }
    }

    stage('test') {
      steps {
        sh 'sudo systemctl start httpd'
      }
    }

  }
}