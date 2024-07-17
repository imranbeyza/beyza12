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
                echo 'Building...'
                bat 'mvn clean install' // bat komutu Windows'ta batch scriptleri için kullanılır
            }
        }
        
        stage('Test') {
            steps {
                echo 'Testing...'
                bat 'mvn test'
            }
        }
        
        stage('Deploy') {
            steps {
                echo 'Deploying...'
                bat 'docker run -d --name myapp myimage:latest' // Docker komutu için bat komutu kullanabilirsiniz
            }
        }
    }
}
