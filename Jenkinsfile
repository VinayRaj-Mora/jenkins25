pipeline {
    agent {
        node {
            label 'Agent-1'
        }
    }
    environment {
        COURSE = "Jenkins for Beginners"
    }
    options{
        timeout(time: 10, unit: 'SECONDS')
        disableConcurrentBuilds()
    }
    stages {
        stage('Build') {
            steps {
                script{
                    sh """
                    echo "Building the project..."
                    echo $COURSE
                    #sleep 10
                    env
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
        aborted {
            echo 'This will run only if the build is aborted'
        }
    }
}