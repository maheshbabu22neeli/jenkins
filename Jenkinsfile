pipeline {
    agent {
        node {
            label 'ROBOSHOP'
        }
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
    post {
        always {
            echo 'I will always says hello world'
        }
        success {
            echo 'Job Success'
        }
        failure {
            echo 'Job Failure'
        }
    }

}