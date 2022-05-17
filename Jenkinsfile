pipeline {
  agent {
    node {
      label 'docker'
    }

  }
  stages {
    stage('Test') {
      parallel {
        stage('Test') {
          steps {
            echo 'Testing'
          }
        }

        stage('Parallel') {
          steps {
            echo 'running in parallel'
          }
        }

      }
    }

    stage('Building') {
      steps {
        echo 'Building'
      }
    }

    stage('Clean up') {
      steps {
        echo 'cleaning'
      }
    }

  }
}