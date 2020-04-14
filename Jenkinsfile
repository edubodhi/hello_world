pipeline{
	agent any
		stages {
			stage ('build') {
				steps {
					echo 'Building the application'
						
					}
				}
		stage ('package') {
				steps {
					def mvnHome= tool name: 'M2_HOME', type: 'maven'
					sh "${mvnHome}/bin/mvn package"
						
					}
				}
	
			stage ('test') {
				steps {
					echo 'Testing the application'
					}
				}
			stage ('deploy') {
				steps {
					echo 'Deploying the application'
					}
				}
			}
		}
