pipeline {
    agent any

    stages {
        stage('Clone Repository') {
            steps {
                git branch: 'main', url: 'https://github.com/Anvesh-ansh259/hello-jenkins.git'
            }
        }

        stage('Show Files') {
            steps {
                sh 'ls -la'
            }
        }
    }
}
