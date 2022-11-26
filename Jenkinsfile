pipeline {
  agent any
  stages {
    stage ('Build') {
      steps {
        echo 'Running build automation'
        sh 'test install'
        archiveArtifacts artifacts: 'webapp/target/*.war',
                   allowEmptyArchive: true,
                   fingerprint: true,
                   onlyIfSuccessful: true
      }
    }
  }
}
