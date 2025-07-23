pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git 'your_repository_url'
            }
        }
        stage('Build') {
            steps {
                sh 'npm install'
                sh 'npm run build' // Or your build command
            }
        }
        stage('Test') {
            steps {
                sh 'npm test'
            }
        }
        stage('Deploy') {
            steps {
                // Add your deployment steps here, e.g., using SSH or Docker
                sh 'echo "Deployment steps go here"'
            }
        }
    }
}
