pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/Praveenamin/testcicd.git'
            }
        }

        stage('Install') {
            steps {
                sh 'npm install'
            }
        }

        stage('Test') {
            steps {
                sh 'npm test'
            }
        }

        stage('Run') {
            steps {
                sh 'node app.js &'
            }
        }
    }
}
