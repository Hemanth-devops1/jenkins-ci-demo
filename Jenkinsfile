pipeline {
    agent any

    stages {

        stage('Checkout Code') {
            steps {
                git branch: 'main',
                url: 'https://github.com/Hemanth-devops1/jenkins-ci-demo.git'
            }
        }

        stage('Build') {
            steps {
                echo "Building project..."
                sh 'ls -la'
            }
        }

        stage('Test') {
            steps {
                echo "Running tests..."
                sh 'echo "No tests yet - learning project"'
            }
        }

    }

    post {
        success {
            echo "Pipeline SUCCESS 🎉"
        }
        failure {
            echo "Pipeline FAILED ❌"
        }
    }
}
