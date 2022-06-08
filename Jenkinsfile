pipeline {
    agent any
    environment {
      docker_cred=credentials('docker-hub')

    }
    stages {
        stage('Build') {
            steps {
              echo $docker_cred_PSW
              echo $docker_cred_USR

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
