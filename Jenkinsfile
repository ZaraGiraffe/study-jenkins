pipeline {
    agent any
    environment {
        PASSWORD = credentials("osboxes_password")
    }
    stages {
        stage('Install apache2') {
            steps {
                script {
                    echo "Install apache2"
                    echo $PASSWORD
                }
            }
        }
    }
}
