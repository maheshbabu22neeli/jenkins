pipeline {
    agent {
        node {
            label 'ROBOSHOP'
        }
    }
    environment {
        project = "roboshop"
        course = "devOps"
    }
    options {
        disableConcurrentBuilds()
        timeout(
            time: 5,
            unit: 'SECONDS'
        )
    }
    stages {
        stage('Build') {
            steps {
                script {
                    sh """
                        echo 'Building..... ${project}'
                        sleep 20
                    """
                }
            }
        }
        stage('Test') {
            steps {
                script {
                    sh """
                        echo 'Testing..... ${project}'
                    """
                }
            }
        }
        stage('Deploy') {
            steps {
                script {
                    sh """
                        echo 'Deploying..... ${project}'
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