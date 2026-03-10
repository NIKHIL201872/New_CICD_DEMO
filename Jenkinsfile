pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/NIKHIL201872/New_CICD_DEMO'
            }
        }

        stage('Build') {
            steps {
                echo "Building application..."
            }
        }

        stage('Test') {
            steps {
                echo "Running tests..."
            }
        }

        stage('Deploy') {
            steps {
                bat '''
                if not exist C:\\deploy-demo mkdir C:\\deploy-demo
                copy file_f1.html C:\\deploy-demo
                '''
            }
        }
    }
}