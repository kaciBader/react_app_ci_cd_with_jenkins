pipeline {
     agent {
        docker {
            image 'node:16-buster-slim'
            args '-p 3000:3000'
        }
    }
    stages {
        stage('Audit') {
            steps {
                echo 'npm audit...'
            }
        }
        stage('build') {
            steps {
                sh 'npm ci'
            }
        }
        stage('Format with Linter') {
            steps {
                echo 'formatting step'
            }
        }
        stage('test') {
            steps {
                echo 'unit tests with jest'
            }
        }
    }
}