pipeline {
    agent {
        docker {
            image 'node:21-alpine'
        }
    }

    stages {
        
        stage('build') {
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
    }
}