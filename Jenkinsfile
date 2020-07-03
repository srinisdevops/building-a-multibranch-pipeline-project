pipeline {
    agent any
    environment {
        CI = 'true'
    }
    stages {
        stage('Build') {
            steps {
                sh 'sudo apt install npm -y'
            }
        }
        stage('Test') {
            steps {

                sh label: '', script: '''pwd
                                        ./jenkins/scripts/test.sh
                                        '''
            }
        }
    }
}
