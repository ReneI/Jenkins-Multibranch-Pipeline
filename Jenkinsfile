pipeline {
	agent any
	environment  { EXECUTE = true
	}
	stages {
		stage('First') {
				
			   when {
                // Only say hello if a "greeting" is requested
                expression { EXECUTE }
            }		    
			
			steps {
				
				sh 'echo "true "'
			}
		}
		stage('Second') { 
			

			   when {
                expression { EXECUTE }
            }
			
			
			steps {
				sh 'echo "updating "'
			}			
		}
		stage('Third') {
			  when {
                expression { EXECUTE= false }
            }
			
			steps {
				sh 'echo "Step Three"'
			}		
		}
	}
}
