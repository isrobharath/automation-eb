pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh "cmake"
                sh 'make'
                sh './hello'
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
