node {
    checkout scm
    docker.image('centos:7.9.2009').withRun('-e CUSTOM_TEXT=hello') { c ->
        sh 'ls'
    }
}
