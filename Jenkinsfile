pipeline {
    agent any
    stages {

         stage('Pull Latest Image') {
            steps {
                 bat "docker pull deepikaarya/mydocker-myimage"
            }
        }
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