pipeline {
    agent  {
        label 'Agent1'
    }
    options {
        
        timeout(time: 30, unit: 'MINUTES')
    }
    parameters {
        string(name: 'PERSON', defaultValue: 'Mr Jenkins', description: 'Who should I say hello to?')

        text(name: 'BIOGRAPHY', defaultValue: '', description: 'Enter some information about the person')

        booleanParam(name: 'TOGGLE', defaultValue: true, description: 'Toggle this value')

        choice(name: 'CHOICE', choices: ['One', 'Two', 'Three'], description: 'Pick something')

        password(name: 'PASSWORD', defaultValue: 'SECRET', description: 'Enter a password')
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
        stage('print parameters')  {
            steps {
                echo "Hello ${params.PERSON}"
                echo "Biography: ${params.BIOGRAPHY}"
                echo "Toggle: ${params.TOGGLE}"
                echo "Choice: ${params.CHOICE}"
                echo "Password: ${params.PASSWORD}"
            }
        }
        }  
        
   }
    
}