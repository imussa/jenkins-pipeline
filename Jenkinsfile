pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }

        stage('Build') {
            steps {
                script {
                    docker.image('centos:7.9.2009') {
                        sh 'uname -a'
                    }
                }
            }
        }
    }

    post {
        success {
            echo "Success."
        }
    }
}
