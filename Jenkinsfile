pipeline {
    agent any

    environment {
    registry = "YourDockerhubAccount/YourRepository"
    registryCredential = 'dockerhub_id'
    dockerImage = ''
    }

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                }
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
