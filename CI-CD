pipeline {
    agent any 
    tools {
        'Maven 3'
    }
    stages {
        stage('Checkout') {
            steps {
                echo 'Kode berhasil di-checkout' 
            }
        }
        stage('Build') {
            steps {
                echo 'Melakukan proses build...'
                // Contoh: sh 'npm install' atau sh 'mvn package'
            }
        }
        stage('Test') {
            steps {
                echo 'Menjalankan unit tests...'
                // Contoh: sh 'npm test' atau sh 'mvn test'
            }
        }
        stage('Deployment') {
            steps {
                echo 'Deployment aplikasi ke server...'
                // Contoh: sh 'scp target/app.jar user@server:/var/www/app'
            }
        }
    }
    post {
        always {
            // Langkah pasca-build
            echo 'Pipeline Selesai.'
        }
        success {
            echo 'Pipeline Berhasil!'
        }
        failure {
            echo 'Pipeline Gagal!'
        }
    }
}
