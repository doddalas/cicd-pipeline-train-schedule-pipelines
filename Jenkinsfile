pipeline {
  agent any
  stages {
    stage ('Build') {
      steps {
        echo 'In Build Step -> Running build automation'
        sh './gradlew build --no-daemon'
        archiveArtifacts artifacts: 'dist/trainSchedule.zip'
      }
    }
  }
}
