pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Building...'
        sh 'echo \'Testing 2\''
      }
    }

    stage('Test Firefox') {
      parallel {
        stage('Test Firefox') {
          steps {
            sh 'echo \'Testing Firefox\''
          }
        }

        stage('Test Chrome') {
          steps {
            sh 'echo \'Testing Chrome\''
          }
        }

        stage('Test Edge') {
          steps {
            sh 'echo \'Testing Edge\''
          }
        }

        stage('Test123') {
          steps {
            sh 'echo \'Test test\''
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        echo 'Deploy'
      }
    }

  }
}