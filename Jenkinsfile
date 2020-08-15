pipeline {
  agents any
  stages {
     stage ('Build') {
       steps {
         echo 'Running build environment'
         sh './gradlew build --no-daemon'
         archiveArtifacts artifacts: 'dist/trainSchedule.zip'
       }
     }
  }
}
