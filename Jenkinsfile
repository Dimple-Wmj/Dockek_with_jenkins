pipeline {
	agent none
	stages {
		stage('Test') {
			agent { 
				docker { image 'busybox' }
			} 
			steps {
				sh ' cat /etc/os-release'
			}
		}
		stage('Test-1') {
			agent {
				docker { image 'alpine' }
			}
			steps {
				sh 'cat /etc/os-release'
			}			
		}
	}
}
