pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Step into build'
      }
    }

    stage('Test') {
      parallel {
        stage('Test') {
          steps {
            echo 'Step into test'
          }
        }

        stage('Coex Tests') {
          steps {
            echo 'Step into Coex Tests'
          }
        }

      }
    }

  }
}