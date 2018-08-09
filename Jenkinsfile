node (label: 'linux') {
    checkout scm

    docker.image('node:alpine').inside {
        sh 'node --version'
    }
}