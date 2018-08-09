pipeline {
    agent {
        docker { image 'node:alpine' }
    }

    stages {
        stage('install') {
            agent {
                label "linux"
            }
            steps {
                sh 'yarn install'
            }
        }

        stage('build') {
            agent {
                label "linux"
            }
            steps {
                sh 'yarn build'
            }
        }

        stage('lint') {
            agent {
                label "linux"
            }
            steps {
                sh 'yarn lint'
            }
        }
    }
}
