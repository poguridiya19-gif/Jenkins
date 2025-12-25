pipeline {
    agent {
        node {
            label 'AGENT-1'
        }
    }
    stages {
        stage('Hello') {
            steps {
               echo "hello world"
            }
        }
        stage('Test') {
            steps {
                echo "Testing"
            }
        }
        stage('Deploy') {
            steps {
                echo "Deploying"
            }
        }
    }
}