pipeline {
	agent any 	
	stages {
		stage('Checkout') {
			steps {
				echo 'Checkout completed'
			}
		}
		stage('Static-test') {
			steps {
				echo 'static tests on code'
			}
		}
		stage('Build') {
			steps {
				sh 'echo "Building the code"'
			}
		}
		stage('Deploy') {
		    when {
                branch 'prod'
            }
			steps {
				echo 'Deploying into environment'
			}
		}
	}
}
