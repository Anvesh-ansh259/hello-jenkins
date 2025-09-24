pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/YOUR-USERNAME/hello-jenkins.git'
            }
        }
        stage('Build') {
            steps {
                sh 'echo "Building project..."'
            }
        }
        stage('Test') {
            steps {
                sh 'echo "Running tests..."'
            }
        }
        stage('Deploy') {
            steps {
                sh '''
                mkdir -p /tmp/jenkins-deploy
                cp index.html /tmp/jenkins-deploy/
                echo "Deployed index.html to /tmp/jenkins-deploy"
                '''
            }
        }
    }
}

