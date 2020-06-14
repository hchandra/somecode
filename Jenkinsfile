pipeline {
  agent {
    label "master"
  }
  trigger {
    cron('H/15 * * * *')
  }
  stages {
    stage('echo') {
      steps {
        echo 'Hello: from trigger'
      }
    }
  }
}
