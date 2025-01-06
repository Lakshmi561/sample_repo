pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                echo "Pulling the code from Git repository"
                git url: 'https://github.com/example-repo/my-app.git', branch: 'main'
            }
        }

        stage('Build') {
            steps {
                echo "Building the application"
                sh 'echo "Building..."'
            }
        }

        stage('Test') {
            steps {
                echo "Running tests"
                sh 'echo "Running tests..."'
            }
        }

        stage('Deploy') {
            steps {
                echo "Deploying the application"
                sh 'echo "Deploying..."'
            }
        }
    }

    post {
        success {
            echo "Pipeline executed successfully!"
        }
        failure {
            echo "Pipeline execution failed!"
        }
    }
}
