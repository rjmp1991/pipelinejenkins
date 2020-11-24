pipeline {
  agent any
  stages {
    stage('stage1') {
      parallel {
        stage('stage1') {
          steps {
            sh 'echo "hola desde el primer stage" > hola.txt'
          }
        }

        stage('stage2') {
          steps {
            echo 'Hola desde stage 2'
          }
        }

        stage('stage 3') {
          steps {
            echo 'hola desde stage 3'
          }
        }

      }
    }

    stage('test') {
      steps {
        sh 'cat hola.txt'
      }
    }

  }
}