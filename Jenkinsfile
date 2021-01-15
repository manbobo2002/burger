pipeline {
    agent any
    environment { 
        CI = 'true'
    }
    stages {
        stage("build") {
            steps {
                nodejs('Node-15.6.0'){
                    sh 'npm install'
                }
            }
        }

        stage("test") {
            steps {
                echo 'testing the app'
            }
        }

        stage("deploy") {
            steps{
                nodejs('Node-15.6.0'){
                    sh 'npm start'
                }
            }
        }
    }
}