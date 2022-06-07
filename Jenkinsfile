pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                docker images
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
