pipeline {
    agent any

    stages {
        stage('Build') {
            when {
                branch 'feature/*'
            }
            steps {
                echo 'Building..'
            }
        }
        stage('Test') {
            when {
                branch 'feature/*'
            }
            steps {
                echo 'Testing...'
            }
        }
        stage('Develop Deploy') {
            when {
                branch 'develop'
            }
            steps {
                echo 'Deploying to Develop....'
            }
        }
        stage('Perf Deploy') {
            when {
                branch 'main'
            }
            steps {
                echo 'Deploying to Perf Environment....'
            }
        }
    }
}