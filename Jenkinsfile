pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                docker.withRegistry( '', registryCredential ) {
                 echo "Testing...."
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
