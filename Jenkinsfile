pipeline {
    agent {
        node {
            label 'Agent-1'
        }
    }
    stages {
        stage('Build') {
            steps {
                script{
                    sh """
                    echo "Building the project..."
                    """
                }
            }
        }
        stage('Test') {
            steps {
                script{
                    sh """
                    echo "Building the project..."
                    """
                }
            }
        }
        stage('Deploy') {
            steps {
                script{
                    sh """
                    echo "Building the project..."
                    """
                }
            }
        }
    }
    post{
        always {
            echo 'This will always run'
            cleanWs()
        }
        success {
            echo 'This will run only if the build succeeds'
        }
        failure {
            echo 'This will run only if the build fails'
        }
    }
}