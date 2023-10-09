def userId
pipeline {
    agent any
    stages {
        stage('Example') {
            steps {
                //echo "Running ${env.BUILD_ID} on ${env.JENKINS_URL}"
            	userId = env.BUILD_USER_ID
            	echo userId
            }
        }
    }
}
