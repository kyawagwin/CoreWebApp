stage('compile') {
  node {
    checkout scm
    stash 'everything'
    dir('CoreWebApp') {
      bat 'dotnet restore'
      bat "dotnet build"
    }
  }
}