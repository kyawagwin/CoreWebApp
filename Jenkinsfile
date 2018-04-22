pipeline {
  agent any
  stages {
    stage('test') {
      steps {
        dir(path: 'CoreWebApp') {
          sh 'docker -v'
        }

        echo 'Hello World!'
      }
    }
  }
  environment {
    PATH = '/usr/local/bin'
  }
}