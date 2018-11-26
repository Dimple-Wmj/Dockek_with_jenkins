pipeline {
    agent {
         docker { image 'nginx:alpine' }
    }
    stages {
	stage('Test') {
		steps {
			sh 'ps -elf | grep nginx'
	     	}
	}
	}
}
