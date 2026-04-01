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
                sh 'mkdir -p deploy'
                sh 'cp index.html deploy/'
            }
        }

        stage('Deploy') {
            steps {
                echo "Deployment stage completed"
            }
        }
    }
}
