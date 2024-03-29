pipeline {
    agent any
	environment {
		PATH = "C:/.NET & Java Software/apache-maven-3.9.6/bin;${env.PATH}"}
    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }
        stage('Build') {
            steps {
				echo "$PATH"
                bat 'mvn clean package'
            }
        }
        stage('Test') {
            steps {
                bat 'mvn test'
            }
        }
    }
}
