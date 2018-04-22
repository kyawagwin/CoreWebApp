pipeline {
  agent {
    dockerfile {
      filename 'CoreWebApp/dockerfile'
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