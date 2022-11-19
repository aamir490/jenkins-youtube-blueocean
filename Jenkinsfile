pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        sh '''pwd
date
ls
ls -a'''
      }
    }

    stage('test') {
      parallel {
        stage('test') {
          steps {
            echo 'this is v8'
          }
        }

        stage('test part') {
          steps {
            echo 'this is b9'
          }
        }

      }
    }

    stage('deploy') {
      steps {
        echo 'deploymennt'
        sleep 10
      }
    }

  }
}