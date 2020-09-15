pipeline {
  agent any
  stages {
    stage('Build') {
      parallel {
        stage('Build1') {
          steps {
            echo 'Building..'
          }
        }

        stage('Build2') {
          steps {
            sh 'echo "Build2"'
          }
        }

        stage('Build3') {
          steps {
            echo 'Build3'
          }
        }

      }
    }

    stage('Test') {
      steps {
        echo 'Testing..'
      }
    }

    stage('Deploy') {
      steps {
        echo 'Deploying....'
      }
    }

  }
}