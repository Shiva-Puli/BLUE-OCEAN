pipeline {
  agent any
  stages {
    stage('Devlopment') {
      parallel {
        stage('Devlopment') {
          steps {
            echo 'DEV stage'
          }
        }

        stage('Unit Testing') {
          steps {
            echo 'Unit test'
          }
        }

      }
    }

    stage('QA') {
      steps {
        echo 'TEST'
      }
    }

    stage('Build') {
      steps {
        echo 'build stage'
      }
    }

    stage('Deployment') {
      parallel {
        stage('Deployment') {
          steps {
            echo 'Deployment'
          }
        }

        stage('Release') {
          steps {
            echo 'Release'
          }
        }

      }
    }

  }
}