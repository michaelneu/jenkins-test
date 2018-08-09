pipeline {
    agent {
        label "linux"
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
