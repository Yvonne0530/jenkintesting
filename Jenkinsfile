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

        stage('Java') {
          steps {
            bat(script: 'java --version', returnStatus: true)
          }
        }

        stage('Git') {
          steps {
            bat(script: 'git --version', returnStatus: true)
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        sleep 5
      }
    }

    stage('Publish') {
      steps {
        writeFile(file: 'result.txt', text: 'Complete !')
      }
    }

  }
}