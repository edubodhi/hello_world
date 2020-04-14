node{
	stage('SCM Checkout'){
		git 'https://github.com/edubodhi/hello_world.git'
	}
		stage ('Compile-package') {
					def mvnHome =  tool name: 'M2_HOME', type: 'maven'
					sh "${mvnHome}/bin/mvn package"
						
					}
		stage ('Deploy') {
					def mvnHome1 =  tool name: 'M2_HOME', type: 'maven'
					sh "${mvnHome1}/bin/mvn deploy"
						
					}
				}
