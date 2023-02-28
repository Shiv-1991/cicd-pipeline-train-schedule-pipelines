pipeline {
  agent any
  stages {
    stage ('Build') {
      steps {
        echo 'The name of stage is: Running Build Automation'
        sh './gradlew build --no-daemon'
        archiveArtifacts artifacts: 'dist/trainSchedule.zip'
      }
    }
  }
}
