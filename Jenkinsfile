pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh "npm install"
                sh "npm run build"
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                 sh 'rm -r /usr/share/nginx/www'
                 sh 'mkdir /usr/share/nginx/www'
                 sh 'cp -r ${WORKSPACE}/build/  /usr/share/nginx/www'
                 

            }
        }
    }
}

