pipeline {
    agent any
    
    stages {
        stage('Clone Repository') {
            steps {
                echo 'Cloning repository...'
                git branch: 'main', url: 'https://github.com/imranbeyza/beyza12.git'
            }
        }
        
     
        stage('Build') {
            steps {
                echo 'Building with Gradle...'
                bat 'gradle clean build'
            }
        }
        
        stage('Test') {
            steps {
                echo 'Running tests...'
                bat 'gradle test'
            }
        }
        
        stage('Deploy') {
            steps {
                echo 'Deploying...'
                sh 'docker run -d --name myapp myimage:latest'
            }
        }
    }
}
