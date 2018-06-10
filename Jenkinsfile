pipeline {
  agent any
  stages {
    stage('Build') {
      parallel {
        stage('Build') {
          steps {
            echo 'HAHA!'
          }
        }
        stage('') {
          steps {
            openshiftDeploy 'mongodb'
          }
        }
      }
    }
  }
}