pipeline {
    agent any
    
    tools {
        jdk 'jdk11'
        maven 'maven3'
    }

    stages {
        stage('Git CLone ') {
            steps {
                git branch: 'qa', url: 'https://github.com/Raghava0684/Shopping-Cart-project.git'
            }
        }
        
        stage('mvn compile ') {
            steps {
                sh 'mvn clean compile -DskipTests=true'
            }
        }
        
        stage('mvn package ') {
            steps {
                sh 'mvn clean package -DskipTests=true'
            }
        }
        
        
    }

}
