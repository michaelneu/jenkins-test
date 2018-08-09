pipeline {
    agent {
        docker { image 'node:alpine' }
    }
    stages {
        stage('build') {
            steps {
                sh 'yarn build'
            }
        }
        stage('lint') {
            steps {
                sh 'yarn lint'
            }
        }
    }
}