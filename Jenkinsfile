pipeline {
    agent any

    stages {

        stage('Git Checkout') {
            steps {
                dir('C:\\GitFiles') {
                    deleteDir()
                    checkout scm
                }
            }
        }

        stage('Verify Files') {
            steps {
                bat '''
                    echo ==========================
                    echo Git files pulled
                    echo ==========================
                    dir C:\\GitFiles
                '''
            }
        }
    }
}