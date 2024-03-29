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
                powershell 'mvn clean package'
            }
        }
        stage('Test') {
            steps {
                powershell 'mvn test'
            }
        }
    }
}
