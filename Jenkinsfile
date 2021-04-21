pipeline{
	agent any
	stages {
		stage('compile Stage'){
			steps {
				withMaven(maven : 'maven_3.6.3'){
					sh 'mvn clean compile'
				}
		
			}
		}
		
		stage('Build Stage'){
			steps {
				withMaven(maven : 'maven_3.6.3'){
					sh 'mvn build'
				}
		
			}
		}
	}
	
	
}