pipeline {
    agent any
    stages {
        stage("Run Test") {
            steps {
                bat "docker-compose-up"
            }
        }
        stage("Bring Grid Down") {
            steps {
                script {
                	bat "docker -compose down"
                }
            }
	}
}
 }      