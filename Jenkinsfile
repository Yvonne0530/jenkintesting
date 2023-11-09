pipeline {
  agent {
    node {
      label 'blueTesting'
    }

  }
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