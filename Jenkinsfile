pipeline {
    agent any

    stages {

        stage('Clone Code') {
            steps {
                git 'https://github.com/CursedSinceBirth-hub/jenkins_exp3.git'
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
