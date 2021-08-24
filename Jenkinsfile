pipeline {
  environment {
    registry = "9515246808/myapp:latest"
    registryCredential = docker hub
  }
 
  any agent
  
  stages {
   
    stage('build image') {
      steps{
        script {
          docker.build registry + ":docker build -t 9515246808/myapp:latest ."
        }
      }
    }
  }
}
