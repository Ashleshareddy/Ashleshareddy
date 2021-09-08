pipeline {
    agent any
    stages {
        stage('Build') {
            agent none
           
            {
              docker {
                    image 'jenkins:2.60.3'
                   
             reuseNode true
                }
            }
            steps {
                sh 'jenkins --version'
           
            }
        }
    }
}
