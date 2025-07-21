pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building...'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing...'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying...'
            }
        }
    post {
        success {
            emailext ( to: 'runrajarun31@gmail.com', subject: 'Pipeline Fail Status', body: "The pipeline got failed")
        }
    failure{
        emailext ( to: 'runrajarun31@gmail.com', subject: 'Pipeline Fail Status', body: "The pipeline got failed" )
            }   
        }
    }
}
