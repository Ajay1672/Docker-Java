pipeline {
    agent any

    stages {

        stage('Clone Repository') {
            steps{
              git branch: 'master', credentialsId: 'a', url: 'git@github.com:Ajay1672/Docker-Java.git'
            }
        }

        stage('clean') {
            steps{
               bat 'cd webApp1 && mvn clean'
            }
        }

        steps {
                // Navigate to webApp1, clean, and package
                bat 'cd webApp1 && mvn package'
            }
}
}
