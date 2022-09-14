pipeline {
    agent any
    environment {
        hi="Hello Class"
    }
    stages {
        stage('Test') {
            steps {
                sh '''
                echo $hi;
                '''
            }
        }
        stage('Deploy') {
            steps {
                sh '''
                chmod +x server.sh
                ./server.sh
                '''
            }
        }
    }
}