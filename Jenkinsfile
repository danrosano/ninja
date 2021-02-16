pipeline {
  agent any
  stages {
    stage('Hola mundo') {
      steps {
        echo 'Hola mundo'
        sh 'echo "Hola ${minombre}"'
      }
    }

    stage('Crear archivo') {
      steps {
        writeFile(file: 'archivo.txt', text: 'Texto del archivo')
        archiveArtifacts '*.txt'
      }
    }

    stage('Despedida') {
      steps {
        input(message: 'Lastima que terminó', ok: 'Excelente taller')
      }
    }

  }
  environment {
    minombre = 'Daniel'
  }
}