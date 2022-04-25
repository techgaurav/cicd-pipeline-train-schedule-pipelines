pipeline {
   agent any
  stages{
    stage ('build'){
      steps{
        echo 'Running build'
        sh './gradlew build --no-daemon'
        rchiveArtifacts artifacts: dist/trainSchedule.zip
      }
    }
  }
}
