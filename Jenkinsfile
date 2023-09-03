// Declarative //
pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
            }
        }
        steps {
            sh 'python unit-test.py'
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
