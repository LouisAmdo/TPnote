pipeline {
    agent any
    
    tools {
        maven 'maven'
    }

    stages {
        stage('Build the Application') {
            steps {
                git credentialsId: 'ceb7a51c-c9d4-40d6-b25c-9895351baaa6', url: 'https://github.com/LouisAmdo/TPnote.git'
                bat 'mvn clean install'
            }
        }
    }
}

