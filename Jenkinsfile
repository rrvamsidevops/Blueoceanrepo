pipeline {
  agent any
  stages {
    stage('Stage1') {
      steps {
        echo 'Stage1'
      }
    }

    stage('Stage2a') {
      parallel {
        stage('Stage2a') {
          steps {
            echo 'Hi Stage2a'
            echo 'Stage2a step2'
          }
        }

        stage('Stage2B') {
          steps {
            echo 'Hello2B'
          }
        }

      }
    }

    stage('Stage3') {
      steps {
        echo 'Stage3 Hello'
      }
    }

  }
}