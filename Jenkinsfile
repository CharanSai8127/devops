pipeline {
    agent any
    
    tools {
        jdk 'jdk 17'
        maven 'maven'
    }

    stages {
        stage('Git-Checkout') {
            steps {
                git 'https://github.com/CharanSai8127/BoardgameListingWebApp.git'
            }
        }
        
        stage('Compile') {
            steps {
                sh 'mvn compile'
            }
        }
        
        stage('Test') {
            steps {
                sh 'mvn test'
            }
        }
        
        stage('Build') {
            steps {
                sh 'mvn package'
            }
        }
        
        
    }
}
