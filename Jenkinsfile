pipeline {
  agent none

  environment {
    APP_NAME = readProperties(file: 'config.ini')['APP_NAME']
  }

  stages {
    stage('Setup') {
      agent any

      steps {
        echo "Setup complete or ${APP_NAME}"
      }
    }
  }
}


