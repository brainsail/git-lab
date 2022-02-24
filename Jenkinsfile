pipeline {
    agent any

    environment {

    }

    stages {

        stage (Lint) {
            when {
                branch 'feature/*'
            }
            steps {
                echo "Linting All The Things!"
            }   
        }

        stage (Build) {
            when {
                branch 'feature/* main'
            }
            steps {
                echo "Build Things!"
            }
        }
    }
}