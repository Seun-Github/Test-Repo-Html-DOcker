pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo 'Building the application...'
                // Example build command
                sh './build.sh'
            }
        }
        stage('Test') {
            steps {
                echo 'Running tests...'
                // Example test command
                sh './run-tests.sh'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying the application...'
                // Example deploy command
                sh './deploy.sh'
            }
        }
    }
}
