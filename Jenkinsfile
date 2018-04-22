pipeline {
  agent {
    node {
      label 'compile'
    }

  }
  stages {
    stage('compile') {
      steps {
        dir(path: 'CoreWebApp') {
          bat 'dotnet restore'
          bat 'dotnet build'
        }

      }
    }
  }
}