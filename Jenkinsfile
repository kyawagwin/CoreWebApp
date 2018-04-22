pipeline {
  agent {
    dockerfile {
      filename 'docker-compose.yml'
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