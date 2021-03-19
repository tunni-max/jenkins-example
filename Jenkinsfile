pipeline {
	agent {  label 'wind-node' }
	stages {
		stage('---clean---'){
			steps {
				tool name: 'maven', type: 'maven'
				sh "mvn clean"
			}
		}
		stage('---test---') {
			steps {
				tool name: 'maven', type: 'maven'
				sh "mvn test"
			}
		}
		stage('---package---'){
			steps {
				tool name: 'maven', type: 'maven'
				sh "mvn package"
			}
		}
	}
}
