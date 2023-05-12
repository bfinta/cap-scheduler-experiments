pipeline {
  agent {
    node {
      label 'linux-docker-18'
    }

  }
  stages {
    stage('a') {
      steps {
        sh 'ls'
      }
    }

    stage('e') {
      steps {
        sh 'ls'
      }
    }

    stage('b') {
      parallel {
        stage('b') {
          steps {
            sh 'ls'
          }
        }

        stage('c') {
          steps {
            sh 'ls'
          }
        }

      }
    }

    stage('d') {
      steps {
        sh 'ls'
      }
    }

  }
}