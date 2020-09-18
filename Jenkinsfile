pipeline {
	agent none
	stages {
		agent { label 'node3' }
		stage ('STAGE 1') {
			steps {
				echo 'This is node3 node with STAGE 1'
				sh 'sleep 10'
			}	
		}
		stage ('STAGE 2') {
			steps {
				echo 'This is slaveforjava with STAGE 2'
				sh 'sleep 10'
			}	
		}
	}
}
