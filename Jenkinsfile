stage('Build') {
    node (label: 'linux') {
        checkout scm

        docker.image('node:alpine').inside {
            sh 'yarn install'
            sh 'yarn build'
        }
    }
}

stage('Lint') {
    node (label: 'linux') {
        checkout scm

        docker.image('node:alpine').inside {
            sh 'yarn install'
            sh 'yarn lint'
        }
    }
}
