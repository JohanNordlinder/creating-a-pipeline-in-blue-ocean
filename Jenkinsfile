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
        stage('Trigger deployment of mongodb') {
          steps {
            openshiftDeploy 'mongodb'
          }
        }
      }
    }
  }
}