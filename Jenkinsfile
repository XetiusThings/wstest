pipeline {
	agent any

	options {
		checkoutToSubdirectory(GetProjectNameFromJobName(JOB_NAME))
	}
	
	stages {
		stage('Winning') {
			steps {
					echo "Repository is now checked out in the subdirectory " + GetProjectNameFromJobName(JOB_NAME)
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
