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

      }
    }

    stage('') {
      steps {
        sh 'cat hola.txt'
      }
    }

  }
}