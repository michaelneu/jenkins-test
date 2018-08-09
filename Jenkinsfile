node {
    label "linux"
    checkout scm

    docker.image('mysql:5') { c ->
        sh 'node --version'
    }
}