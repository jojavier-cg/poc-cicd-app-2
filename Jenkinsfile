pipeline {
	agent any

	stages {

			stage('Build Application') {
				steps {
					sh 'mvn verify org.sonarsource.scanner.maven:sonar-maven-plugin:sonar -Dsonar.projectKey=jojavier-cg_poc-cicd-app-2 -Dsonar.sources=. -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=31a3d88ba3a215e9174804cb002f87c2a2ae3064 -Dsonar.organization=jojavier-cg'
				}
			}
	}
}
