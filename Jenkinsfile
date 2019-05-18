pipeline {
	  agent any
	      stages {
		        stage ('sonar') {
			steps {
				      withSonarQubeEnv('SonarPipeline') {
					      withMaven(maven: 'My-Maven') {
						      sh 'mvn clean install sonar:sonar'
					    }
				}
			}

		}
	}
}
