pipeline {
    agent any
    environment {
        NIAM_CRED = credentials('MY-CRED')
    }
    parameters {
        string(
            name: 'VERSION',
            defaultValue: '1.0',
            description: 'Application version'
        )
    }

    stages {
        stage('Build') {
            steps {
                echo "Version: ${params.VERSION}"
            }
        }
    }


    stages {
        stage('Hello') {
            steps {
                sh '''
                echo NIAM USERNAME : $NIAM_CRED_USR
                echo NIAM PASSWORD : $NIAM_CRED_PSW
                '''
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

