pipeline {
    agent any

    stages {

        stage('Clone') {
            steps {
                echo "Cloning repository..."
            }
        }

        stage('Build') {
            steps {
                echo "Building project..."
            }
        }

        stage('Prepare Deployment') {
            steps {
                bat '''
                if not exist deploy mkdir deploy
                copy /Y index.html deploy\\
                '''
            }
        }

        stage('Deploy') {
            steps {
                echo "Deployment completed successfully"
            }
        }
    }
}