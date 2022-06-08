pipeline {
    agent any

    

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                docker.withRegistry('docker-hub', registryCredential ) {
                  echo "docker registery"
                }
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
