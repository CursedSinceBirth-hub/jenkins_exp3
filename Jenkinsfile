pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo "Building project..."
                bat '"C:\Users\Sarthak Deochake\AppData\Local\Python\pythoncore-3.14-64\python.exe" app.py'
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
