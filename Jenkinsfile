pipeline {
  agent none

  environment {
    APP_NAME = 'hello-world'
  }

  stages {
    stage('Setup') {
      agent any

      steps {
        echo "Inside stage setup"
      }
    }
  }
}


