pipeline{
	agent any
	stages {
		stage('compile Stage'){
			steps {
					sh 'mvn clean compile'
			}
		}
		
		stage('Build Stage'){
			steps {
					sh 'mvn build'
			}
		}
	}
	
	
}