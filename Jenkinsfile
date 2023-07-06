pipeline {
  agent any
  stages {
    stage('dev') {
      steps {
        echo 'this is devlpement stage'
      }
    }

    stage('test') {
      steps {
        echo 'this is testing'
      }
    }

    stage('build') {
      parallel {
        stage('build') {
          steps {
            echo 'this is build stage'
          }
        }

        stage('fixes') {
          steps {
            echo 'this is fixes stage'
          }
        }

        stage('prod') {
          steps {
            echo 'this is production stage'
          }
        }

        stage('deploy') {
          steps {
            echo 'this is deployment stage'
          }
        }

      }
    }

  }
}