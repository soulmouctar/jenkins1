pipeline {
    agent any

    environment {
        MY_VAR = 'my_value'
        MY_NUMBER = 42
    }

    stages {
        
        stage('Deploy') {
            steps {
                echo "BRANCH_NAME ${env.BRANCH_NAME}"
                echo "BRANCH_IS_PRIMARY ${env.BRANCH_IS_PRIMARY}"
                echo "CI ${env.CI}"
                echo "BUILD_NUMBER ${env.BUILD_NUMBER}"
                echo "JENKINS_URL ${env.JENSKINS_URL}"
                echo "MY_NUMBER ${env.MY_NUMBER}"
                echo 'printenv'
            }
        }
    }
}