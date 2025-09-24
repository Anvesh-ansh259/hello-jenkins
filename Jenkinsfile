pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                git branch: 'main',
                    url: 'https://github.com/Anvesh-ansh259/hello-jenkins.git',
                    credentialsId: '0a513b4c-6947-45fb-b94c-86c29611e680'
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
