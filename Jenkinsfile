pipeline {
  agent {
    node {
      label '1604'
    }

  }
  stages {
    stage('test') {
      parallel {
        stage('test') {
          agent any
          steps {
            sleep 5
            echo 'test'
          }
        }
        stage('test2') {
          agent any
          steps {
            sleep 10
          }
        }
      }
    }
    stage('final') {
      steps {
        echo 'DONE'
      }
    }
  }
}