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
    }
}
post {
    success {
        emailext ( replyTo: 'runrajarun31@gmail.com', subject: 'Pipeline Status', to: 'runrajarun31@gmail.com')
    }
}
