pipeline {
    agent any
    environment {
        PASSWORD = credentials("osboxes_password")
    }
    stages {
        stage('Install apache2') {
            steps {
                sh 'echo "Install apache2"'
                sh 'echo $PASSWORD'
            }
        }
    }
}
