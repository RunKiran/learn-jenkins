pipeline {
    agent {
        label 'Agent1'
    }
    options {
        
        timeout(time: 1, unit: 'SECONDS')
    }
    stages {
        stage('Build') {
            steps {
                sh 'echo This is BUILD'
            }
        }
        stage('TEST') {
            steps {
                sh 'echo This is TEST'
                sh 'sleep 10'
            }
        }
        stage('Deploy') {
            steps {
                sh 'echo This is Deploy'
            }
        }
    }
}