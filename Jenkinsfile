pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'SCM checkout..'
				checkout scm
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
