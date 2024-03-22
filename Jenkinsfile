pipeline {
    agent any 
    stages {
        stage('Audit') {
            steps {
                echo 'npm audit...'
            }
        }
        stage('dependances installation') {
            steps {
                echo 'npm ci'
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