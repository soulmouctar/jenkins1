pipeline {
    agent any
    // agent {
    //     docker {
    //         image 'node:21-alpine'
    //         args '-u root:root'
    //     }
    // }

    triggers {
        cron('* * * * *')
    }

    stages {
        // stage('Check npm') {
        //     steps { sh 'npm -v' }
        }
        
        stage('build') {
            steps {
                echo 'Hello World'
            }
        }
    }

    // post {
    //     always {
    //         echo 'Pipeline completed.'
    //     }
    //     success {
    //         echo 'Pipeline succeeded.'
    //     }
    //     failure {
    //         echo 'Pipeline failed.'
    //     }
    // }
}