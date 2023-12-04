pipeline {
  agent any
  stages {
    stage('development') {
      steps {
        echo 'dev stage'
      }
    }

    stage('QA') {
      steps {
        echo 'qa stage'
      }
    }

    stage('testing') {
      steps {
        echo 'testing stage'
      }
    }

    stage('deploy') {
      parallel {
        stage('deploy') {
          steps {
            echo 'deploy stage'
          }
        }

        stage('production') {
          steps {
            echo 'prod stage'
          }
        }

        stage('service') {
          steps {
            echo 'service stage'
          }
        }

      }
    }

  }
}