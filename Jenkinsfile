stage('Build') {
    node (label: 'linux') {
        docker.image('node:alpine').inside {
            sh 'yarn install'
            sh 'ls -lha'
            sh 'yarn build'
        }
    }
}

stage('Lint') {
    node (label: 'linux') {
        docker.image('node:alpine').inside {
            sh 'yarn install'
            sh 'yarn lint'
        }
    }
}
