pipeline {
    agent {
        label 'AGENT-1'
    }
    options {
        // Timeout counter starts AFTER agent is allocated
        timeout(time: 1, unit: 'SECONDS')
        disableConcurrentBuilds()
    }
    stages {
        stage('Build') {
            steps {
                echo 'Building..'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
                //sh 'sleep 10'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}