pipeline {
  agent any
  stages {
    stage('Plan') {
      steps {
        echo 'i have to plan to work on cicd'
      }
    }

    stage('code') {
      steps {
        echo 'extrate code from version control'
      }
    }

    stage('build') {
      parallel {
        stage('build') {
          steps {
            echo 'building the code'
          }
        }

        stage('test') {
          steps {
            echo 'i want to test '
          }
        }

        stage('release') {
          steps {
            echo 'i want to release'
          }
        }

        stage('Deploy') {
          steps {
            echo 'deploying '
          }
        }

        stage('operate') {
          steps {
            echo 'i want to operate'
          }
        }

      }
    }

  }
}