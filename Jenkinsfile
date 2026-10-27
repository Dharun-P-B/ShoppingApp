
pipeline {
    agent any

    environment {
        DOCKER = 'C:\\Users\\dharu_naut31y\\AppData\\Local\\Programs\\DockerDesktop\\resources\\bin\\docker.exe'
    }

    stages {
        stage('Checkout Verified') {
            steps {
                echo 'GitHub source was retrieved by Jenkins.'
                echo 'Shopping App - 24MIS0200'
            }
        }

        stage('Check Docker') {
            steps {
                bat '"%DOCKER%" --version'
            }
        }

        stage('Build Docker Image') {
            steps {
                bat '"%DOCKER%" build -t dharunpb/shoppingapp:v1 .'
            }
        }
    }
}
