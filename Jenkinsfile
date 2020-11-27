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
        stage('Coex Tests') {
          steps {
            echo 'Step into Coex Tests'
          }
        }

        stage('Offline Regression Tests') {
          steps {
            echo 'Step into Offline Regression Tests'
          }
        }

        stage('Online Regression Tests') {
          steps {
            echo 'Step into Online Regression Tests'
          }
        }

      }
    }

  }
}