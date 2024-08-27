pipeline {
    agent { 
        node {
            label 'docker-agent-linux'
            }
      }
    triggers {
        pollSCM '* * * * *'
    }
    stages {
        stage('Build') {
            steps {
                echo "Building 2rd time.."
                sh '''
                echo "Building something"
                '''
            }
        }
        stage('Test') {
            steps {
                echo "Testing 2rd time.."
                sh '''
                echo "Testing something"
                '''
            }
        }
        stage('Deliver') {
            steps {
                echo 'Deliver 2rd time.'
                sh '''
                echo "Deliver stuff.."
                '''
            }
        }
    }
}