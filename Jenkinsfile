pipeline {
    agent any
    
    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }
        
        stage('Build') {
            steps {
                // Projeyi derlemek için gerekli komutları buraya ekleyin
                // Örneğin:
                // sh 'mvn clean package'
                // veya
                // bat 'gradle build'
            }
        }
        
        stage('Test') {
            steps {
                // Testleri çalıştırmak için gerekli komutları buraya ekleyin
                // Örneğin:
                // sh 'mvn test'
                // veya
                // bat 'gradle test'
            }
        }
        
        stage('Deploy') {
            steps {
                // Uygulamayı hedef ortama dağıtmak için gerekli komutları buraya ekleyin
                // Örneğin:
                // sh 'kubectl apply -f deployment.yaml'
                // veya
                // bat 'deploy.cmd'
            }
        }
    }
    
    post {
        success {
            // Başarı durumunda yapılacak işlemleri buraya ekleyin
            // Örneğin:
            // echo 'Başarıyla tamamlandı!'
        }
        failure {
            // Başarısızlık durumunda yapılacak işlemleri buraya ekleyin
            // Örneğin:
            // echo 'Hata oluştu!'
        }
    }
}
