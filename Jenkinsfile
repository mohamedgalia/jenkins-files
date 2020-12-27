pipeline {
	agent any
	stages {

        stage('Code Checkout') {
		  steps {
            git 'https://github.com/nadergan/jenkins-java.git'
		  }
		}

		stage('Build') {
            steps {
                sh 'mvn clean compile'
		    }
		}
		
		stage('Test') {
            steps {
                sh 'mvn test'
            }
        }


	}
}
