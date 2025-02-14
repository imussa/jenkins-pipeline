pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                docker.build('myalpine')
            }
        }
    }
}
