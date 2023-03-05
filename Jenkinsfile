pipeline {
  agent any
  stages {
    stage('Test') {
      parallel {
        stage('Test') {
          steps {
            echo 'Code Testing'
          }
        }

        stage('Test Par') {
          steps {
            echo 'Redundant Code'
          }
        }

      }
    }

    stage('Build') {
      steps {
        sh '''pwd
hostname
date
cal 2023'''
      }
    }

    stage('Deploy') {
      steps {
        echo 'Deployment Successfull'
        sleep 10
      }
    }

  }
}