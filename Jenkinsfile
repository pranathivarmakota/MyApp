pipeline {
    agent any
    environment{
        PATH = "C:/Users/e040107/Downloads/apache-maven-3.9.8-bin/apache-maven-3.9.8/bin;${env.PATH}"
    }

    stages {
        stage('Checkout') {
            steps {
                git "https://github.com/pranathivarmakota/MyApp.git"
            }
        }
        stage('Test'){
            steps{
                bat "mvn test"
            }
        }
        stage('install'){
            steps{
                bat "mvn install"
            }
        
        }
    }
}

