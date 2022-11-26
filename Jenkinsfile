pipeline {
  agent any
  stages {
    stage ('Build') {
      steps {
        echo 'Running build automation'
        sh 'test install'
        archiveArtifacts artifacts: 'test/webapp/target/webapp.war', followSymlinks: false
      }
    }
  }
}
