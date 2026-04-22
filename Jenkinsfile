pipeline {
    agent any

    stages {
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
