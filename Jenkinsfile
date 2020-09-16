pipeline {

	agent any
	tools {
		maven 'maven'
	}
	stages {
		stage ('Compile Stage') {
			steps {
				bat 'mvn clean compile'
			}
		}
		stage ('Sonarqube deployement Stage') {
			steps {
				bat 'mvn sonar:sonar'
			}
		}
		stage ('Test') {
			steps {
				bat 'mvn test'
			}
		}
	}
}
