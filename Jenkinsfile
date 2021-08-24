pipeline {
  environment {
    registry = "docker push 9515246808/myapp:tagname"
    registryCredential = ‘https://hub.docker.com/_/jenkins’
  }
  agent any
  stages {
    stage('Cloning Git') {
      steps {
        git 'https://github.com/gustavoapolinario/microservices-node-example-todo-frontend.git'
      }
    }
    stage('build image') {
      steps{
        script {
          docker.build registry + ":$BUILD_NUMBER"
        }
      }
    }
  }
}
