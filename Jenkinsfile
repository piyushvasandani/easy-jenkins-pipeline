pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh '''pwd 
ls 
echo "Hello world"'''
      }
    }

    stage('Test') {
      parallel {
        stage('Test') {
          steps {
            echo 'Testing is done'
          }
        }

        stage('test param') {
          steps {
            sh '''pwd
ls
echo "this is test parameter"'''
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        sleep 10
      }
    }

  }
}