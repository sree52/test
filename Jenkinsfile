pipeline {
    agent any

    environment {
        docker-hub = credentials('docker-hub')
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
