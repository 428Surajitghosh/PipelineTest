//def userId
pipeline {
    agent any
    stages {
        stage('Example') {
            steps {
                //echo "Running ${env.BUILD_ID} on ${env.JENKINS_URL}"
            	wrap([$class: 'BuildUser']) {
                    echo "userId=${BUILD_USER_ID}"
                    }
            }	
        }
    }
}
