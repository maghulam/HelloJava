pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        withGradle()
      }
    }

    stage('Copy Artifact') {
      steps {
        archiveArtifacts(artifacts: '*.war', fingerprint: true)
      }
    }

  }
}