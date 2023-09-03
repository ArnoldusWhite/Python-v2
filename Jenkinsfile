// Declarative //
pipeline {
    agent any

    stages {
        stage('Build') {
            steps {  
                  bat 'pip install -r requirements.txt'
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
