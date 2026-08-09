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
                sh 'echo Build Successful'
            }
        }

        stage('Test') {
            steps {
                echo 'Running tests...'
                sh 'echo All Tests Passed'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying application...'
                sh 'echo Deployment Successful'
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
