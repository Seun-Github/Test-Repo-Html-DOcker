pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo 'Building the application...'
                // Example build command
                sh 'docker build -t jenkinsimage .'
            }
        }
        stage('Test') {
            steps {
                echo 'Running tests...'
                sh '''
                docker tag jenkinsimage shawn4dockerhub/jenkinsimage
                docker login -u "shawn4dockerhub" -p "just4Udocker"
                docker push shawn4dockerhub/jenkinsimage
                '''
  
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying the application...'
 
            }
        }
    }
}
