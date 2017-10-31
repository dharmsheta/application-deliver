pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        step([$class: 'CopyArtifact', projectName: 'dharmsheta/application-build/master'])
        archiveArtifacts artifacts: '*.sh', fingerprint: true
      }
    }
  }
}
