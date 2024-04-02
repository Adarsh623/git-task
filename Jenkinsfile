pipeline {
    agent any
    stages {
        stage('java') {
            steps {
                sh ' java --version'
            }
        }
        stage('python install') {
            steps {
                sh ' sudo apt install python3 -y '
            }
        }
        stage('check python3') {
            steps {
                sh ' python3 --version '
            }
        }
        stage('install apche') {
            steps {
                sh 'sudo apt update'
                sh 'sudo apt install apache2 -y'
                sh 'sudo systemctl status apache2'
                sh 'sudo systemctl start apache2'
            }
        }
    }
}
