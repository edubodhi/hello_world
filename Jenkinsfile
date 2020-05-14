node{
		stage('Git Login'){
				  git 'https://github.com/edubodhi/hello_world.git'
				   }
		stage ('Compile-package') {
					def mvnHome =  tool name: 'M2_HOME', type: 'maven'
					sh "${mvnHome}/bin/mvn package"
						
					}
		stage ('Install') {
					def mvnHome1 =  tool name: 'M2_HOME', type: 'maven'
					sh "${mvnHome1}/bin/mvn install"
						
					}
	        stage ('docker -push') {
					docker.withRegistry('https://registary.hub.docker.com', 'docker-hub)
				        def imagepush = docker.build('prahi001/webapp')
				            imagepush.push()
							    }
				}
