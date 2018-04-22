pipeline {
  agent any
  stages {
    stage('test') {
      steps {
        dir(path: 'CoreWebApp') {
          sh '''docker -v

done'''
        }

        echo 'Hello World!'
      }
    }
  }
  environment {
    PATH = '/usr/bin:/usr/local/bin'
  }
}