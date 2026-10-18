pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                echo 'Getting source code from GitHub'
                checkout scm
            }
        }

        stage('Build') {
            steps {
                echo 'Building the application'
                sh 'echo Build completed successfully'
            }
        }

        stage('Test') {
            steps {
                echo 'Testing the application'
                sh 'echo All tests passed'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deployment stage completed'
                sh 'echo Application deployment demo successful'
            }
        }
    }

    post {
        success {
            echo 'Pipeline completed successfully!'
        }

        failure {
            echo 'Pipeline failed. Check the console output.'
        }
    }
}
