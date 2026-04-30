pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'echo "Building..."'
            }
        }

        stage('Test') {
            steps {
                sh 'echo "Testing..."'
            }
        }

        stage('Deploy') {
            steps {
                sh 'echo "Deploying..."'
            }
        }
    }

    post {
        always {
            echo 'This will always run (success or failure)'
        }
        success {
            echo 'Build succeeded '
        }
        failure {
            echo 'Build failed '
        }
        unstable {
            echo 'Build is unstable '
        }
        changed {
            echo 'Build status changed from last run'
        }
    }
}