pipeline {
    agent any
    environment {
        PASSWORD = credentials("osboxes_password")
    }
    stages {
        stage('Install apache2') {
            steps {
                sh 'echo $PASSWORD | sudo -S apt install -y apache2'
            }
        }
    }
}
