pipeline {
  agent {
    label 'master'
  }
  stages {
    stage('build') {
      steps {
        awsCodeBuild credentialsType: 'keys', downloadArtifacts: 'false', projectName: 'sls-jenkins-small', region: 'us-east-1', sourceControlType: 'jenkins'
      }
    }
  }
}
