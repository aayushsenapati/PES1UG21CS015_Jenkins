pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'g++ hello.cpp -o hello // Replace with your actual compilation command
            }
        }
        stage('Test') {
            steps {
                sh './hello' // Replace with your actual execution command
            }
        }
        stage('Deploy') {
            echo 'Deploying...'
        }
    }

    post {
        success {
            echo 'Pipeline succeeded!'
        }
        failure {
            echo 'Pipeline failed!'
        }
    }
}
