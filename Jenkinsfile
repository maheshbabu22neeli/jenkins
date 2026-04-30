pipeline {
    agent any
    options {
        // Timeout counter starts AFTER agent is allocated
        timeout(time: 1, unit: 'SECONDS')
    }
    stages {
        stage('Build') {
            steps {
                script {
                    sh """
                        echo 'Building.....'
                    """
                }
            }
        }
        stage('Test') {
            steps {
                script {
                    sh """
                        echo 'Testing.....'
                    """
                }
            }
        }
        stage('Deploy') {
            steps {
                script {
                    sh """
                        echo 'Deploying.....'
                    """
                }
            }
        }
    }

}