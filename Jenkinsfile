pipeline {
agent amy
stages {
  stage ('Build') {
    steps {
    echo 'Running build automation'
    ssh './gradlew build --no-daemon'
    archiveArtifacts artifacts: 'dist/trainSchedule.zip'
    }
   }
  }
}
