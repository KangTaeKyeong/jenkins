pipeline {
  agent any
  stages {
    stage('buile') {
      steps {
        sh 'echo "Hello world"'
      }
    }

    stage('test') {
      parallel {
        stage('test') {
          steps {
            sh '''sudo yum install -y httpd
sudo systemctl start httpd'''
          }
        }

        stage('test-1') {
          steps {
            sh 'ls -al'
          }
        }

      }
    }

  }
}