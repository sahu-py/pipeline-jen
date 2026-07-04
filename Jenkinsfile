pipeline {
    agent any
    environment {
        NIAM_CRED = credential('MY-CRED')

    stages {
        stage('Hello') {
            steps {
                echo 'NIAM USERNAME : $MYE-CRED_USR'
                echo 'NIAM PASSWORD : $MYE-CRED_PSW'
            }
        }
        stage('hi') {
            steps {
                 sh 'date'
            }
        }
        stage('bye') {
            steps {
                echo 'i am done'
            }
        }
        }
    }

