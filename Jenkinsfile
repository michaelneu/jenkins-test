pipeline {
    agent {
        docker { image 'node:alpine' }
    }
    stages {
        stage("Clone") {
            steps {
                checkout scm
            }
        }
        
        stage('Test') {
            steps {
                sh 'node --version'
            }
        }
    }
}