pipeline {
  agent any
  stages {
    stage('stage1') {
      parallel {
        stage('stage1') {
          steps {
            sh 'echo "hola"'
          }
        }

        stage('stage2') {
          steps {
            echo 'Hola desde stage 2'
          }
        }

      }
    }

  }
}