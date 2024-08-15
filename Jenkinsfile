pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh "gcc hello.c -o hello"
                sh "./hello"
                echo 'Building..'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}