pipeline {
  agent any
  stages {
    stage('Echoing Messages') {
      steps {
        sh 'echo "Hello Ankit Sambhare here!!!!" > result.txt'
      }
    }

    stage('Post') {
      steps {
        archiveArtifacts 'result.txt'
      }
    }

  }
  triggers {
    cron('H/15 * * * *')
  }
}