
pipeline {
    agent any

    stages {
        stage('Checkout Verified') {
            steps {
                echo 'GitHub source was retrieved by Jenkins.'
                echo 'Shopping App - 24MIS0200'
            }
        }

        stage('Build Docker Image') {
            steps {
                bat 'docker --version'
                bat 'docker build -t dharunpb/shoppingapp:v1 .'
            }
        }
    }
}
