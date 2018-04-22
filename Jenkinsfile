pipeline {
  agent {
    docker {
      image 'microsoft/aspnetcore:2.0'
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