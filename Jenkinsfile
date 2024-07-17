pipeline {
    agent any
    stages {
        stage('Checkout SCM') {
            steps {
                checkout scm
            }
        }
        stage('Build') {
            steps {
                // Build komutlarını buraya ekleyin
                sh 'mvn clean install'
            }
        }
        stage('Test') {
            steps {
                // Test komutlarını buraya ekleyin
                sh 'mvn test'
            }
        }
        stage('Deploy') {
            steps {
                // Deploy komutlarını buraya ekleyin
                sh 'mvn deploy'
            }
        }
    }
}
