pipeline {
    agent {
         docker { 
		image 'nginx:alpine'
		args '-v /root/wmj:/usr/share/nginx/html'
         }

    }
    stages {
	stage('Build') {
		steps {
			sh 'apk add --no-cache curl openssl'
		}
	}
        stage('Test') {
        	steps {
			sh 'curl localhost/abc.html'
		}
	}
    }
}
