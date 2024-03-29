pipeline {
    agent any
	environment {
		PATH = "C:/.NET & Java Software/apache-maven-3.9.6/bin;C:/.NET & Java Software/openjdk17/bin;${env.PATH}"
	}
    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }
        stage('Build') {
            steps {
				bat 'mvn -v'
				bat 'java --version'
				echo "$PATH"
                //bat 'mvn clean package'
            }
        }
        stage('Test') {
            steps {
				echo "asd"
                //bat 'mvn test'
            }
        }
    }
}
