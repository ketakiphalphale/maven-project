pipeline {
	  agent any
	      stages {
		        stage ('sonar') {
			steps {
				      withSonarQubeEnv('Sonarjob1') {
					      withMaven(maven: 'LocalMaven') {
						      sh 'mvn clean install sonar:sonar'
					    }
				}
			}

		}
	}
}
