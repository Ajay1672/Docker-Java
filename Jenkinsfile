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
}
}
