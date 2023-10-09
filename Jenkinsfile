def userId
pipeline {
    agent any
    stages {
        stage('Example') {
            steps {
                //echo "Running ${env.BUILD_ID} on ${env.JENKINS_URL}"
            	userId = $BUILD_USER_ID
            	echo userId
            }
        }
    }
}
