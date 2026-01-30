pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }

        stage('Build & Test') {
            steps {
                bat 'mvn clean test'
            }
        }

        stage('Deploy') {
            steps {
                bat 'scripts\\deploy.bat'
            }
        }
    }
}
