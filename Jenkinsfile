pipeline {
    agent {
        node {
            label 'AGENT-1'
        }
    }
    environment {
        COURSE = "Jenkins" 
    }
    // this is build section
    stages {
        stage('Build') {
            steps {
               script{
                sh """
                    echo "Building"
                    echo $COURSE
                """
               }
            }
        }
        stage('Test') {
            steps {
               script{
                sh """
                    echo "Building"
                """
               }
            
            }
        }
        stage('Deploy') {
            steps {
                script{
                  sh """
                      echo "Building"
                  """
                }
            }
        }
    }
    post{
        always{
            echo 'i will always say hello again !'
            cleanWs()
        }
    }
}
