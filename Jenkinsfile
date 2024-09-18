pipeline {
  agent any

  stages {
    stage ('checkout') {
      steps {
        //pulling the upgraded source code //
        git 'https://github.com/JKP1008shine/docker-cicd.git'
      }
    }

    stage ('build') {
      steps {
        script {
          //build the docker image//
          sh 'make image'
        }
      }
    }
    
    stage ('test') {
      steps {
        script {
          //testing the app//
          sh 'make test'
        }
      }
    }

    stage ('deploy') {
      steps {

      }
    }
  


  }
}
