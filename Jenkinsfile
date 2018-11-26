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
        	steps {
			sh 'curl localhost/abc.html'
		}
	}
    }
}
