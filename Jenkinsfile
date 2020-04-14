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
					sh 'mvn package'
						
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
