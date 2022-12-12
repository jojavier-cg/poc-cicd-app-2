pipeline {
	agent any

	stages {

			stage('Build Application') {
				steps {
					sh 'mvn verify org.sonarsource.scanner.maven:sonar-maven-plugin:sonar -Dsonar.projectKey=jojavier-cg_poc-cicd-app-2'
				}
			}
	}
}
