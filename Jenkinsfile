pipeline {
    agent any
    environment {
        PASSWORD = credentials("osboxes_password")
    }
    stages {
        stage('Install apache2') {
            steps {
                sh 'echo $PASSWORD | sudo apt install apache2'
            }
        }
    }
}
