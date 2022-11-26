pipeline {
  agent any
  stages {
    stage ('Build') {
      steps {
        echo 'Running build automation'
        sh 'clean install'
        archiveArtifacts artifacts: 'webapp.war'
      }
    }
  }
}
