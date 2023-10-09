import groovy.json.JsonSlurper

//def userId
pipeline {
    agent any
    stages {
        stage('Select User') {
            steps {
                //echo "Running ${env.BUILD_ID} on ${env.JENKINS_URL}"
            	wrap([$class: 'BuildUser']) {
               		echo "userId=${BUILD_USER_ID}"
				}
				def users=readJSON file: "${env.WORKSPACE}\\users.json"
				JsonSlurper slurper = new JsonSlurper()
				Map parsedJson=slurper.parseText(users)
				echo "token=${parsedJson.get("1")}"
            }	
        }
    }
}
