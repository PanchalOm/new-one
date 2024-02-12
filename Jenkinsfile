pipeline {
  agent any
  stages {
    stage('build') {
      parallel {
        stage('build') {
          steps {
            echo 'this is the basic build stage'
          }
        }

        stage('build2') {
          steps {
            sleep 5
          }
        }

      }
    }

    stage('test') {
      steps {
        echo 'testing stage'
      }
    }

    stage('deploy') {
      steps {
        echo 'deploy the data'
      }
    }

  }
}