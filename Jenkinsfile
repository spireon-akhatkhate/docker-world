def loadProperties() {
    node {
        checkout scm
        properties = readProperties file: 'config.ini'
        echo "Read config.ini file"
    }
}

pipeline {
  agent none

  stages {

    stage ('prepare') {
        agent any

        steps {
            script {
                loadProperties()
                echo "App Name - ${properties.APP_NAME}"
            }
        }
    }

    stage('Setup') {
      agent any

      steps {
        echo "Inside stage setup"
      }
    }
  }
}


