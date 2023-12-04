pipeline {
	agent any 
	parameters {
		choice(name: 'ENVIRONMENT', choices: ['QA','UAT'], description: 'Pick Environment value')
	}
	stages {
	    stage('Checkout') {
	        steps {
			checkout scm			       
		      }}
		stage('Deployment'){
		   steps {
		sh 'cp target/myntra.war /home/dev/Downloads/apache-tomcat-9.0.82/webapps'
			}}	
}}
