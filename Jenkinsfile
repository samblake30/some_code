pipeline {
  agent any
  stages {
    stage('Echoing Messages') {
      steps {
        echo 'hello'
        echo 'hello from the trigger'
      }
    }

  }
  triggers {
    cron('H/15 * * * *')
  }
}