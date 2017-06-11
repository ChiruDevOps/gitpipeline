pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                echo 'SCM checkout..'
				checkout scm
            }
        }
        stage('Build') {
            steps {
		call bat 'nant --buildfile:hudson.build'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
