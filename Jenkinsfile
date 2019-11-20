pipeline {
    // master executor should be set to 0
    agent any
    stages {
        stage('Pull Latest Image') {
            steps {
                //sh
                bat "docker pull cmeatarun1988/selenium-docker"
            }
        }
        stage('Execute Scripts') {
            steps {
                //sh
                bat "docker-compose up hub chrome firefox"
            }
        }
        stage('Execute Scripts') {
            steps {
                //sh
                bat "docker-compose up search-module book-flight-module"
            }
        }
    }
}