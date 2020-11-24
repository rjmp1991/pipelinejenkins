pipeline {
  agent any
  stages {
    stage('stage1') {
      steps {
        sh 'echo "Actualizando Hola.txt" > hola.txt'
        sh 'cat hola.txt'
      }
    }

    stage('stage2') {
      steps {
        sh 'echo "append file step2" >> hola.txt'
      }
    }

  }
}