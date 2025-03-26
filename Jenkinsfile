pipeline {
    agent any

    tools {
        maven 'Maven'  // The name given in Global Tool Configuration
    }
    
    stages {
        stage('Build') {
            steps {
                bat 'echo Building the project...'
            }
        }

        stage('Test') {
            steps {
                echo 'Running tests...'
                bat 'mvn test'  // Ensure Maven is accessible
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying the application...'
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
