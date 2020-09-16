pipeline {

	agent any
	tools {
		maven 'maven'
	}
	stages {
		stage ('Compile Stage') {
			steps {
				sh 'mvn clean compile'
			}
		}
		stage ('Sonarqube deployement Stage') {
			steps {
				sh 'mvn sonar:sonar'
			}
		}
		stage ('Test') {
			steps {
				sh 'mvn test'
			}
		}
	}
}
