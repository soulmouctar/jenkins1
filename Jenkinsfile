pipeline {
    agent {
        docker {
            image 'node:21-alpine'
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