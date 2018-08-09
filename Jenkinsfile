pipeline {
    agent {
        label "linux"
    }

    stages {
        stage('install') {
            agent {
                docker { image 'node:alpine' }
            }
            steps {
                sh 'yarn install'
            }
        }

        stage('build') {
            agent {
                docker { image 'node:alpine' }
            }
            steps {
                sh 'yarn build'
            }
        }

        stage('lint') {
            agent {
                docker { image 'node:alpine' }
            }
            steps {
                sh 'yarn lint'
            }
        }
    }
}
