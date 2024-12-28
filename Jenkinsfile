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
        stage('Get errors') {
            sh 'grep \'HTTP/1.1" [45][0-9][0-9] \' /var/log/apache2/access.log'
        }
    }
}
