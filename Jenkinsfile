pipeline {
    agent any
    
    tools {
        maven 'maven-3.8.3' 
    }

    stages {
        
        stage('fetching the code') {
            steps {
                git credentialsId: 'github-cred', url: 'https://github.com/vin58dev/hackathon-starter.git'
            }
        } 
        stage('build the code') {
            steps {
                sh 'mvn clean package'
            }
        }
        
     
    }
}
