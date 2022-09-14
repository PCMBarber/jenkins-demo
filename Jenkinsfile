pipeline {
    agent any
    stages {
        stage('Test') {
            steps {
                sh '''
                echo 'doing tests';
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