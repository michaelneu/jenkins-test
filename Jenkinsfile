pipeline {
    agent {
        docker { image 'node:alpine' }
    }

    stages {
        stage('install') {
            steps {
                sh 'yarn install'
            }
        }

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