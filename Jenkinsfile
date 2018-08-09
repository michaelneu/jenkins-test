pipeline {
    agent {
        label 'linux'
    }

    stages {
        stage('foo') {
            steps {
                sh 'docker run --rm node:alpine node --version'
            }
        }
    }
}
