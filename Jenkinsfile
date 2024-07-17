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
               steps {
        echo 'Building...'
        sh 'mvn clean install'
            }
        }
        stage('Test') {
            steps {
        echo 'Testing...'
        sh 'mvn test'
        }
        stage('Deploy') {
            steps {
                echo 'Deploying...'
                sh 'docker run -d --name myapp myimage:latest'
            }
        }
    }
}
