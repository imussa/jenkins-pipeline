pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                script {
                    docker.build('myalpine')
                }
            }
        }
    }
}
