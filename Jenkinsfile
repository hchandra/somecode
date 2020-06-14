pipeline {
  agent {
    label "master"
  }
  triger {
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
