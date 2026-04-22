pipeline {
    agent any

    stages {

        stage('Clone Code') {
            steps {
                git 'https://github.com/your-username/exp3-jenkins-pipeline.git'
            }
        }

        stage('Build') {
            steps {
                echo "Building project..."
                bat 'python app.py'
            }
        }

        stage('Test') {
            steps {
                echo "Testing project..."
                bat 'python -m py_compile app.py'
            }
        }

    }
}