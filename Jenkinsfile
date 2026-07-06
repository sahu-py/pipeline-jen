pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building Application'
            }
        }

        stage('Tests') {
            parallel {

                stage('Unit Test') {
                    steps {
                        echo 'Running Unit Tests'
                    }
                }

                stage('Integration Test') {
                    steps {
                        echo 'Running Integration Tests'
                    }
                }

                stage('Security Scan') {
                    steps {
                        echo 'Running Security Scan'
                    }
                }
            }
        }
    }
}
