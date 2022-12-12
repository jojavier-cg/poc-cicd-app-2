pipeline {
	agent any

	stages {

			stage('Build Application') {
				steps {
					sh 'mvn clean install'
				}
			}
			
			stage('Test') {
				steps {
					echo 'Application in Testing Phase…'
					sh 'mvn -v'
					sh 'java -version'
					sh 'mvn test'
				}
			}		
			
			stage('Deploy to Server') {
				steps {
					echo 'Deploying mule project due to the latest code commit…'
					echo 'Deploying to the configured environment….'
					sh 'mvn clean package deploy -DmuleDeploy'
				}
			}
		
	}
}
