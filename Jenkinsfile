pipeline {
    agent {
        docker {
            image 'node:24-alpine3.21'
            args '-u root:root'
        }
    }

    stages {
        
        stage('Deploy') {
            steps {
                sh 'npm -v'
            }
        }
    }

    post {
        always {
            echo 'Pipeline completed.'
        }
        success {
            echo 'Pipeline succeeded.'
        }
        failure {
            echo 'Pipeline failed.'
        }
    }
}