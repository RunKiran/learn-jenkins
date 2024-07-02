pipeline {
    agent {
        label 'Agent1'
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
            }
        }
        stage('Deploy') {
            steps {
                sh 'echo This is Deploy'
            }
        }
    }
}