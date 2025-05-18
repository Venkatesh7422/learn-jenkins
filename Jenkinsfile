pipeline {
    agent {
        node {
            label 'agent-1'
    }
    }
    //build
    stages {
        stage('Build') {
            steps {
                echo 'Building..'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
    //psot build
      post { 
        always { 
            echoI' will always say Hello again!'
        }
        failure{
            echo 'this runs when pipeline is failed, used generally to send some alerts'
        }
        success{
            echoI 'I will say Hello, when pipeline is success'
        }
    }
}
