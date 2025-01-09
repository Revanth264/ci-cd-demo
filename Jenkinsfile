pipeline {
    agent any
    stages {
        stage('Clone Repository') {
            steps {
                git branch: 'main', url: 'https://github.com/Revanth264/ci-cd-demo.git'
            }
        }
        stage('Build') {
            steps {
                sh 'pytest tests/'
            }
        }
        stage('Test') {
            steps {
                sh '''
                    . venv/bin/activate
                    echo "Running tests (placeholder)"
                '''
            }
        }
        stage('Deploy') {
            steps {
                sh '''
                    . venv/bin/activate
                    echo "Deploying application..."
                '''
            }
        }
    }
}

