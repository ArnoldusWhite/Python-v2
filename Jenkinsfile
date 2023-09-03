// Declarative //
pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                withEnv(['PATH+EXTRA=/usr/sbin:/usr/bin:/sbin:/bin']) {  
                  sh 'pip install -r requirements.txt'
                }
            }
        }
        stage('Test'){
            steps {
                sh 'python test.py'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
