pipeline {
	agent any
	environment  { EXECUTE: TRUE
	}
	stages {
		stage('Stage 1') {
				
			   when {
                // Only say hello if a "greeting" is requested
                expression { EXECUTE }
            }		    
			
			steps {
				
				sh 'echo "true "'
			}
		}
		stage('Stage 2') { 
			

			   when {
                expression { EXECUTE }
            }
			
			
			steps {
				sh 'echo "updating "'
			}			
		}
		stage('Stage 3') {
			  when {
                expression { EXECUTE==FALSE }
            }
			
			steps {
				sh 'echo "Step Three"'
			}		
		}
	}
}
