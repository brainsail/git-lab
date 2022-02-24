pipeline {
    agent any

    stages {

        stage ('Lint') {
            when {
                branch 'feature/*'
            }
            steps {
                echo "Linting All The Things!"
            }   
        }

        stage ('Build') {
            when {
                branch 'main'
            }
            steps {
                echo "Build Things!"
            }
        }
    }
}