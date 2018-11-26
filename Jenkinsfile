pipeline {
    agent {
//        docker { image 'node:7-alpine' }
         docker { 
		image 'maven:3-alpine'
		args '-v $HOME/.m2:/root/.m2'
         }

    }
    stages {
        stage('Test') {
            steps {
//                sh 'node --version'
		sh 'ls $HOME/.m2'
            }
        }
	stage('Build') {
		sh 'mvn -B'
	}
    }
}
