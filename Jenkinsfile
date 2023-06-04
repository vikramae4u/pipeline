pipeline {
  agent any
  stages {
    stage('Devops') {
      steps {
        echo 'Devlopment stage'
      }
    }

    stage('test') {
      parallel {
        stage('test') {
          steps {
            echo 'testing'
          }
        }

        stage('build') {
          steps {
            echo 'we build code'
          }
        }

        stage('deployement') {
          steps {
            echo 'code deploy'
          }
        }

        stage('operate') {
          steps {
            echo 'execution'
          }
        }

      }
    }

  }
}