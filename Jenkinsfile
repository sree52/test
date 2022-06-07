pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                withCredentials([usernamePassword(credentialsId: 'docker-hub', passwordVariable: 'pass', usernameVariable: 'user')]) {
                    // the code here can access $pass and $user
                  //  echo  $pass
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
