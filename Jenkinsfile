pipeline {
    agent any
    environment {
        NIAM_CRED = credentials('MY-CRED')
    }

    stages {
        stage('Hello') {
            steps {
                echo "NIAM USERNAME : $NIAM_CRED_USR"
                echo "NIAM PASSWORD : $NIAM_CRED_PSW"
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

