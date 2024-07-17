pipeline {
    agent any
    stages {
        stage('Clone Repository') {
            steps {
                git 'https://github.com/imranbeyza/beyza12.git'
            }
        }
        stage('Build') {
            steps {
                echo 'Building...'
                // Buraya build adımlarınızı ekleyin
            }
        }
        stage('Test') {
            steps {
                echo 'Testing...'
                // Buraya test adımlarınızı ekleyin
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying...'
                // Buraya deploy adımlarınızı ekleyin
            }
        }
    }
}
