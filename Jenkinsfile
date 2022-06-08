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
              docker tag sree52/nginx-test:v1  356903330565.dkr.ecr.us-west-2.amazonaws.com/runner:nginx-test
              docker images
              aws ecr get-login-password --region us-west-2 | docker login --username AWS --password-stdin 356903330565.dkr.ecr.us-west-2.amazonaws.com
              docker push 356903330565.dkr.ecr.us-west-2.amazonaws.com/runner:nginx-test


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
