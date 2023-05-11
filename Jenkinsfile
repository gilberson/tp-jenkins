pipeline {
  agent any
  stages {
    stage('stage1') {
      steps {
        sh '''

sudo  apt-get -y update && sudo apt-get -y upgrade'''
      }
    }

    stage('stage2') {
      steps {
        sh 'dpkg -l > /tmp/paquets'
      }
    }

    stage('stage3') {
      steps {
        sh '''\'\'\'
if 
[`grep -c git /tmp/paquets` -ne 0]






then dpkg -s git else sudo apt-get install -y git fi \'\'\''''
      }
    }

  }
}