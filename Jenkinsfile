pipeline {
    agent any

    environment {
        docker-hub = credentials('docker-hub')
    }

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                echo $docker-hub                
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
