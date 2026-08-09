pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                echo 'Checking out source code...'
            }
        }

        stage('Build') {
            steps {
                echo 'Building the application...'
                bat 'echo Build Successful'
            }
        }

        stage('Test') {
            steps {
                echo 'Running tests...'
                bat 'echo All Tests Passed'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying application...'
                bat 'echo Deployment Successful'
            }
        }
    }

    post {
        success {
            echo 'Jenkins Pipeline completed successfully!'
        }

        failure {
            echo 'Jenkins Pipeline failed!'
        }

        always {
            echo 'Pipeline execution completed.'
        }
    }
}
