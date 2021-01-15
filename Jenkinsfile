pipeline {
    agent any
    stages {
        stage("run frontend") {
            steps {
                echo 'executing....'
                nodejs('Node-15.6.0') {
                    sh 'npm install'
                }
            }
        }
        stage("build") {
            steps {
                echo 'building the app....'
                echo 'building the app'
            }
        }

        stage("test") {
            steps {
                echo 'testing the app'
            }
        }

        stage("deploy") {
            steps{
                echo 'deploy the app'
            }
        }
    }
}