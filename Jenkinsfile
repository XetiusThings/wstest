pipeline {
	agent any

	options {
		checkoutToSubdirectory(GetProjectNameFromJobName(JOB_NAME)
	}
	
	stages {
		stage('Winning') {
			steps {
					echo "JOB_NAME : ${JOB_NAME}"
					echo "Winning"
			}
		}
	}
}

def GetProjectNameFromJobName(def jobName) {
    println "jobName : ${jobName}"
    
    if (jobName.contains("/")) {
        parts = jobName.split("/")
        return parts[parts.size() - 2]
    } else {
        return jobName
    }
}
