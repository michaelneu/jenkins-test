pipeline {
    agent {
        docker { image 'node:alpine' }
    }
    stages {
        stage('build') {
            steps {
                sh 'yarn install'
                sh 'yarn build'
            }
        }
        stage('lint') {
            steps {
                sh 'yarn install'
                sh 'yarn lint'
            }
        }
    }
}