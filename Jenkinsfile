pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh "yarn"
                sh "yarn build"
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

