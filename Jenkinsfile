@Library('shared-repo') _

pipeline {
    agent any
    triggers {
        cron('*/2 * * * *')
    }
    stages {
        stage('Test') {
            steps {
                echo 'Initiated Integrated Test Execution'
                script {
                    integrationTest.run()
            }
            }
        }
    }
}
