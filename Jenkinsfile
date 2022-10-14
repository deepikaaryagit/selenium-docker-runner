pipeline {
    agent any
    stages {
        stage('Run Test') {
            steps {
                 bat "docker-compose up"
            }
        }
        stage('Bring Grid Down') {
            steps {
               
                bat "Bring Grid Down"
            }
        }
      
    }
} 