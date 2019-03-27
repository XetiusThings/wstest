pipeline {
	agent any
	stages {
		stage ('Checkout') {
			steps {
				dir('${PROJECT_NAME}') {
					checkout scm
				}
			}
		}
	}
}
