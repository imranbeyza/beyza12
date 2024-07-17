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
               steps
        sh 'mvn clean install'
            }
        }
        stage('Test') {
            steps {
      
        sh 'mvn test'
        }
        stage('Deploy') {
            steps {
               
                sh 'docker run -d --name myapp myimage:latest'
            }
        }
    }
}
