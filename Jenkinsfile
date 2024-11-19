pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/jef0014/pruebas.git'
            }
        }

        stage('Install Dependencies') {
            steps {
                bat 'npm install'
            }
        }

        stage('Run Tests') {
            steps {
                bat 'npm test'
            }
        }
    }
}