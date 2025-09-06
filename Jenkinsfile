pipeline {
    agent any
    // agent {
    //     docker {
    //         image 'node:21-alpine'
    //         args '-u root:root'
    //     }
    // }

    triggers {
        pollSCM('* * * * *')
    }

    stages {
        // stage('Check npm') {
        //     steps { sh 'npm -v' }
        // }
        
        stage('build') {
            steps {
                echo 'Hello World'
            }
        }

         stage('deployment production') {
            input {
                message "Vous voulez vraiment déployer?"
                ok "Yes, let's do it!"
                submitter "admin, soulmouctardev"
                submitterParameter "USER_SUBMIT"
                parameters{
                    string(name: 'VERSION', defaultValue: 'latest', description: 'Une version')
                }
            }
            steps {
                echo 'user ${USER_SUBMIT} has submitted'
                echo "deploiement de la version ${VERSION}"
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