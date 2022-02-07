pipeline {
    agent any

    stages {
        stage('Build Phase') {
            steps {
                echo 'Hello Build'
                bat 'mvn package'
            }
        }
        stage('Test Phase') {
            steps {
                echo 'Hello Test'
                bat 'mvn test -DmuleTest'
            }
        }
        stage ('Deploy Phase'){
	        steps{
	        	echo 'Hello Deploy'
	        	bat 'mvn deploy -DmuleDeploy'
	        }
    }
}
