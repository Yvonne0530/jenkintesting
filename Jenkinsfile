pipeline {
  agent any
  stages {
    stage('Build') {
      parallel {
        stage('Build') {
          steps {
            echo 'On Progress'
          }
        }

        stage('Test') {
          steps {
            echo 'Building'
          }
        }

      }
    }

  }
}