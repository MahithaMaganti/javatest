pipeline {
    agent any
    
    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }
        
        stage('Build') {
            steps {
                echo 'Building the application...'
                // Add your build commands here
                // Example: sh 'mvn clean package'
            }
        }
        
        stage('Test') {
            steps {
                echo 'Running tests...'
                // Add your test commands here
                // Example: sh 'mvn test'
            }
        }
        
        stage('Deploy') {
            steps {
                echo 'Deploying the application...'
                // Add your deployment commands here
            }
        }
    }
    
    post {
        success {
            echo 'Pipeline completed successfully!'
        }
        failure {
            echo 'Pipeline failed!'
        }
    }
}
