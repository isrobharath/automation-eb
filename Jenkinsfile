pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo '*****************************************'
                sh 'mkdir build'
                echo '*****************************************'
                sh 'cd build'
                echo '*****************************************'
                sh "cmake .."
                echo '*****************************************'
                sh 'make'
                echo '*****************************************'
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
