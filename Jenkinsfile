pipeline {
  agent any
  stages {
    stage('stage1') {
      steps {
        sh 'sudo -S apt-get -y update && sudo -S apt-get -y upgrade'
      }
    }

    stage('stage2') {
      steps {
        sh 'dpkg -l > /tmp/paquets'
      }
    }

  }
}