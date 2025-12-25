pipeline {
    // these are pre-build sections
    agent {
        node {
            label 'AGENT-1'
        }
    }
    environment {
        COURSE = "Jenkins" 
    }
    options{
        timeout(time:10,unit:'seconds')
        disableConcurrentBuilds()
    }
    // this is build section
    stages {
        stage('Build') {
            steps {
               script{
                sh """
                    echo "Building"
                    echo $COURSE
                    sleep 10
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
        success{
            echo 'i will run if success'
        }
        failure{
            echo 'i will run if failure'
        }
        aborted{
            echo 'pipeline is aborted'
        }
    }
}
