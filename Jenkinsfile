pipeline {
    agent any

    tools {
        nodejs "nodes"  // Asegúrate de que el nombre coincida con el configurado en Jenkins
    }

    stages {
        stage('Checkout') {
            steps {
                echo 'Obteniendo el código fuente desde el repositorio Git...'
                git 'https://github.com/jef0014/pruebas.git'
            }
        }

        stage('Install Dependencies') {
            steps {
                echo 'Instalando dependencias...'
                bat 'npm install'
            }
        }
        stage('Prueba Unitaria') {
            steps {
        
                bat 'npm test'
            }
        }

       
    }
}