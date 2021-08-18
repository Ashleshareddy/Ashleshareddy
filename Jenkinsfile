pipeline {
  agent any
  stages {
    stage('Stage1') {
      parallel {
        stage('Stage1') {
          steps {
            sh 'echo "First stage"'
          }
        }

        stage('Stage1.1') {
          steps {
            sh 'echo "Parallel stage 1.1"'
          }
        }

      }
    }

    stage('Stage2') {
      steps {
        sh 'echo "2nd Stage "'
      }
    }

    stage('Deploy') {
      steps {
        sh 'echo "Deploy stage"'
      }
    }

  }
}