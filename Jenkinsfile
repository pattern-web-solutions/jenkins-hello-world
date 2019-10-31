pipeline {
    agent {
        node {
            label 'docker'
        }
    }

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
                slackSend channel: "random", message: "3.14159"
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
        stage('Notify') {
            steps {
                slackSend message: "Hello World Job Is Complete"
            }
        }
    }
}