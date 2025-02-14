pipeline {
    agent {
        docker { image 'centos:7.9.2009' }
    }

    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }

        stage('Build') {
            steps {
                docker.image('centos:7.9.2009').inside {
                    sh 'hostname'
                }
            }
        }
    }
}
