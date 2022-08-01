pipeline {
  agent {
    label 'master'
  }
  stages {
    stage('build') {
      steps {
        awsCodeBuild credentialsType: 'keys', downloadArtifacts: 'false', projectName: 'jenkins-small', region: 'eu-central-1', sourceControlType: 'jenkins'
      }
    }
  }
}
