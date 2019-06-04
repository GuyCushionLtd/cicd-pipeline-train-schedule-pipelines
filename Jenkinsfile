pipeline {
  agent any
  stages {
    stage ('Builds') {
      steps {
        echo 'Running build automation'
        sh './gradlew build --no-daemon'
        archiveArtifacts artifacts: dist/trainSchedule.zip
      }
    }
  }
}
