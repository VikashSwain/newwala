pipeline {
  agent none
  stages {
    stage('build') {
      steps {
        sh '''pwd
date'''
      }
    }

    stage('test') {
      parallel {
        stage('test') {
          steps {
            echo 'testing required'
            sh 'pwd'
          }
        }

        stage('test1') {
          steps {
            sh 'pwd'
            echo 'hiii there'
          }
        }

      }
    }

    stage('deploy') {
      steps {
        sleep 20
      }
    }

  }
}