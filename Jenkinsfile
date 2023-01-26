pipeline {
  agent any
  stages {
    stage('dev') {
      steps {
        echo 'i want to print'
      }
    }

    stage('test') {
      parallel {
        stage('test') {
          steps {
            echo 'this is testing'
          }
        }

        stage('deploy') {
          steps {
            echo 'this is gui pipeline'
          }
        }

      }
    }

  }
}