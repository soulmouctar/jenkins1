pipeline {
    agent any

    stages {
        
        stage('Deploy') {
            steps {
                echo "BRANCH_NAME ${env.BRANCH_NAME}"
                echo "BRANCH_IS_PRIMARY ${env.BRANCH_IS_PRIMARY}"
                echo "CI ${env.CI}"
                echo "BUILD_NUMBER ${env.BUILD_NUMBER}"
                echo "JENSKINS_URL ${env.JENSKINS_URL}"
            }
        }
    }
}