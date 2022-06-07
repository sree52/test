pipeline {
    agent any

    environment
      {
        docker-hub = credentials('docker-hub')
      }

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
