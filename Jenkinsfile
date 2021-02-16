pipeline {
  agent any
  stages {
    stage('Hola mundo') {
      steps {
        echo 'Hola mundo'
        sh 'printenv'
      }
    }

    stage('Crear archivo') {
      steps {
        writeFile(file: 'archivo.txt', text: 'Texto del archivo')
      }
    }

  }
}