# terraform
This is a terraform repository
# Pipeline
pipeline {
    agent any
    stages {
        stage('Pull') {
            steps {
                echo 'Pull Success'
            }
        }
        stage('Build') {
            steps {
                sh 'echo \'Application is Build\''
            }
        }
        stage('Test') {
            steps {
                echo 'Test Success'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploy Success'
            }
        }
    }
}
