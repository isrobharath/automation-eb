pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo '*****************************************'
                sh 'rm -rf build'
                echo '*****************************************'
                sh 'mkdir build'
                echo '*****************************************'
                // sh 'cd build'
                echo '*****************************************'
                sh "cmake -B build"
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
