pipeline {
    agent any
    stages {

        stage('Pull Latest Image') {
            steps {
                 bat "docker pull deepikaarya/mydocker-myimage"
            }
        }
        stage('Start Docker Hub with chrome and firefox') {
            steps {
                 bat "docker-compose up -d hub chrome firefox"
            }
        }
        stage('Run Tests') {
            steps {
                 bat "docker-compose up test-module-firefox test-module-chrome"
            }
        }
   

        }
        post{
            always{
                archiveArtifacts artifacts:'outputResults/**'
                   bat "docker-compose down"
            }

        }
      
    }
 