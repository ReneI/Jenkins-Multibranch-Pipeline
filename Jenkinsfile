pipeline {
    agent {
        docker {
            image 'node:6-alpine'
            args '-p 3000:3000 -p 5000:5000' 
        }
    }
    environment {
        CI = 'true'
    }
 
   
	stages {
		stage('One') {
			steps {
				sh 'echo "Step One"'
			}
		}
		stage('Two') { 
			steps {
				sh 'echo "Step Two"'
			}			
		}
		stage('Three') {
			steps {
				sh 'echo "Step Three"'
			}		
		}
	}

