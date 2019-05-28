pipeline {
  agent any
  steps {
    stage ('Build') {
      steps {
        ehco 'Running build automation'
        sh './gradlew build --no-daemon'
        archiveArtifacts artifacts: 'dist/trainSchedule.zip'
      }
    }
  }
}
