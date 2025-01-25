pipeline {
    agent any

    stages {
        stage('Install Dependencies') {
            steps {
                sh 'npm install'
            }
        }
        stage('Run Tests') {
            steps {
                // Comando errado: "npm run tests" em vez de "npm test"
                sh 'npm run tests'
            }
        }
        stage('Build') {
            steps {
                sh 'npm run build'
            }
        }
    }
}
