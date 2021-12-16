pipeline {
    agent any

    stages {
        stage('Build') {
			environment {
				ANYPOINT_CREDENTIALS = credentials('wp.anypoint.credentials')
			}
            
            steps {
                bat "mvn clean install deploy -DmuleDeploy -Dusername=ptiwari104 -Dpassword=Petter942@ -Denvironment=Sandbox -DworkerType=Micro -Dworkers=1 -Dregion=us-east-2"
            }
        }
    }
}