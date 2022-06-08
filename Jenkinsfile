pipeline {
    agent any
    environment {
      docker_cred=credentials('docker-hub')

    }
    stages {
        stage('Build') {
            steps {
            sh """
              env
              docker login -u ${docker_cred_USR} -p ${docker_cred_PSW}
              docker pull sree52/nginx-test:v1
              docker images
             """
              //  echo $docker_cred_PSW
            //  echo $docker_cred_USR

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
