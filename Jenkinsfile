pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Building...'
      }
    }

    stage('Testing Firefox') {
      parallel {
        stage('Testing Firefox') {
          steps {
            sh 'echo "Testing Firefox"'
          }
        }

        stage('Testing chrome') {
          steps {
            sh 'echo "Testing chrome"'
          }
        }

        stage('Testing edge') {
          steps {
            sh 'echo "Testing Edge"'
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        echo 'Deployed'
      }
    }

  }
}