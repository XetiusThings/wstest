pipeline {
	agent any

	options {
		skipDefaultCheckout true
	}
	
	stages {
		stage ('Checkout') {
			steps {
				dir('${currentBuild.projectName}') {
					checkout scm
				}
			}
		}
	}
}
