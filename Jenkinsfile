pipeline {
	agent any
	stages {
		stage('Build') {
			steps {
				bat 'cd monappli & mvn install'
			}
		 post {
                success {
                    junit '**/target/surefire-reports/*.xml'
                        }
                 }
               
		}
	}
}