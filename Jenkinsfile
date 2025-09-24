pipeline {
    agent any

    stages {
        stage('Clone Repository') {
            steps {
                git 'https://github.com/Anvesh-ansh259/hello-jenkins.git'
            }
        }

        stage('Show Files') {
            steps {
                sh 'ls -la'
            }
        }
    }
}
