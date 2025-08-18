pipeline {
    agent any

    environment {
        MY_VAR = 'my_value'
        MY_NUMBER = 42
    }

    stages {
        
        stage('Deploy') {
            steps {
                sh 'npm -v'
            }
        }
    }
}