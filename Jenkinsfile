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
			sh 'curl localhost/abc.html'
		}
	}
    }
}
