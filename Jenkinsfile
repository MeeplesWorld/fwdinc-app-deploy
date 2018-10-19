pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        step([$class: 'CopyArtifact', projectName: 'fwdinc-app-build'])
        archiveArtifacts artifacts: '*.sh', fingerprint: true
      }
    }
  }
}
