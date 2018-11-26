pipeline {
    agent {
         docker { 
		image 'nginx:alpine-curl'
		args '-v /root/wmj:/usr/share/nginx/html'
         }

    }
    stages {
	stage('Build') {
		steps {
			sh 'ps -elf | grep nginx'
		}
	}
        stage('Test') {
        	steps {
			sh 'curl localhost/abc.html'
		}
	}
    }
}
