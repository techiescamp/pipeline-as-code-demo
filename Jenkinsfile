pipeline {
    agent any
    
    environment {
        APP_NAME = "SIMPLE_APP"
    }
    
    stages {
        stage('Stage 1') {
            steps {
                sh """
                    echo "Running Stage 1"
                    echo "Application Name: \${APP_NAME}"
                """
            }
        }
        
        stage('Stage 2') {
            steps {
                sh 'env | sort'
            }
        }
        
        stage('Stage 3') {
            steps {
                sh '''
                    echo "Current directory:"
                    pwd
                    echo "Listing files:"
                    ls -la
                '''
            }
        }
    }
}
