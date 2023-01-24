pipeline {
  agent any
  stages {
    stage('Dev') {
      steps {
        echo 'I want to print'
      }
    }

    stage('Test') {
      parallel {
        stage('Test') {
          steps {
            echo 'I want to Print'
          }
        }

        stage('deploy') {
          steps {
            echo 'I want to Deploy'
          }
        }

      }
    }

  }
}