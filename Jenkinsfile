pipeline {
  agent {
    node {
      label 'master'
    }

  }
  stages {
    stage('web') {
      steps {
        dir(path: 'CoreWebApp') {
          sh 'dotnet restore'
          sh 'dotnet build'
        }

      }
    }
  }
}