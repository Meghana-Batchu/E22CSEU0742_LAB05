pipeline {
    agent any
    
    stages {
        stage('Build') {
           stage('Build') {
            steps {
                bat 'echo Building the project...'
            }
        }

        
        stage('Test') {
            steps {
                echo 'Running tests...'
                sh 'mvn test'
            }
        }
        
        stage('Deploy') {
            steps {
                echo 'Deploying the application...'
                // Add your deployment steps here
            }
        }
    }
    
    post {
        success {
            echo 'Pipeline executed successfully!'
        }
        failure {
            echo 'Pipeline failed. Check the errors!'
        }
    }
}
