pipeline {
    agent any
    environment { 
        CI = 'true'
    }
    stages {
        stage("build") {
            steps {
                sh 'npm install'
            }
        }

        stage("test") {
            steps {
                echo 'testing the app'
            }
        }

        stage("deploy") {
            steps{
                sh 'npm start'
            }
        }
    }
}