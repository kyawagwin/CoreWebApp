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
          bat 'dotnet restore'
          bat 'dotnet build'
        }

      }
    }
  }
}