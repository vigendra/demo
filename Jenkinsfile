pipeline {
  agent any
  stages {
    stage('devp') {
      steps {
        echo 'i want development'
      }
    }

    stage('build') {
      parallel {
        stage('build') {
          steps {
            echo 'i want build'
          }
        }

        stage('Test') {
          steps {
            echo 'i want test'
          }
        }

        stage('deploy') {
          steps {
            echo 'i want deploy'
          }
        }

      }
    }

  }
}