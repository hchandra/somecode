pipeline {
  agent {
    label "master"
  }
  triggers {
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
