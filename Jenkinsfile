pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                // Checkout the code from the repository
                git 'https://github.com/daisyjabbour/D-M.git'
            }
        }

        stage('Build') {
            steps {
                // Your build steps go here
                sh 'mvn clean install'
            }
        }

        stage('Deploy') {
            steps {
                // Your deployment steps go here
                sh './deploy.sh'
            }
        }
    }
}

