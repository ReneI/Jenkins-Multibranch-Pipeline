pipeline {
	agent any
	stages {
		stage('Stage 1') {
			  script {
                    env.variable = "TRUE" {
			
			steps {
				
				sh 'echo "true "'
			}
		}
		stage('Stage 2') { 
			
			   when {
                // Only say hello if a "greeting" is requested
                expression { env.variable == 'TRUE' }
            }
			
			
			steps {
				sh 'echo "updating "'
			}			
		}
		stage('Stage 3') {
			steps {
				sh 'echo "Step Three"'
			}		
		}
	}
}
