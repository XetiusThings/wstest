pipeline {
	agent any

	options {
		checkoutToSubdirectory("directory")
	}
	
	stages {
		stage('Winning') {
			steps {
					sh 'env > env.txt' 
					for (String i : readFile('env.txt').split("\r?\n")) {
    					println i
					}
					echo "Winning"
			}
		}
	}
}
