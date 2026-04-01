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
        bat 'mkdir deploy'
        bat 'copy index.html deploy\\'
            }
        }

        stage('Deploy') {
            steps {
                echo "Deployment stage completed"
            }
        }
    }
}
