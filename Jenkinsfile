pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git 'git@github.com:Khadija-Elabaidi/test_jenkins.git'
            }
        }

        stage('Build') {
            steps {
                bat 'mvn clean compile'
            }
        }

        stage('Test') {
            steps {
                bat 'mvn test'
            }
        }
    }
}