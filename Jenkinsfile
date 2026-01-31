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
                bat 'C:\\Program Files\\Apache\\Maven\\apache-maven-3.9.12\\bin'
            }
        }

        stage('Deploy') {
            steps {
                bat 'scripts\\deploy.bat'
            }
        }
    }
}
