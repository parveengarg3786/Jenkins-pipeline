pipeline {
	agent any
	stages {
		stage('compile Stage'){
			steps {
					sh 'mvn clean compile'
			}
		}
		
		stage('Deployment Stage'){
			steps {
					sh 'mvn clean deploy -DmuleDeploy -DskipTests -Dmule.version=4.3.0 -Danypoint.username=praveen_TMC -Danypoint.password=QWERasdf1234 -Denv=Sandbox -Dappname=Jekins-pipeline -Dbusiness=TechMatrix-Sandbox -DvCore=Micro -Dworkers=1'
			}
		}
		
		stage('Deployment to second environment'){
			steps {
					sh 'mvn deploy -DmuleDeploy -DskipTests -Dmule.version=4.3.0 -Danypoint.username=praveen_TMC -Danypoint.password=QWERasdf1234 -Denv=UAT -Dappname=Jekins-pipeline -Dbusiness=TechMatrix-Sandbox -DvCore=Micro -Dworkers=1'
			}
		}
	}
	
	
}
