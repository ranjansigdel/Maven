pipeline {
    agent any
    tools {
        maven 'MAVEN_HOME'
    }
    
    stages {
        stage('Welcome Master Branch') {
            steps {
                echo 'Welcome to Jenkins Pipeline'
            }            
        }
        stage('Checkout') {
            steps {                
                git 'https://github.com/ranjansigdel/DEVOPS-B25.git'
            }
        }
        stage('Clean Stage') {
            steps {
                sh 'mvn clean'
            }            
        }
        stage('Test Stage') {
            steps {
                sh 'mvn test'
            }            
        }
        stage('Pre-Build Stage') {
            steps {
                echo 'This is Pre-Build Stage'
            }            
        }
        stage('Build Stage') {
            steps {
                sh 'mvn install'
            }            
        }
        stage('Post-Build Stage') {
            steps {
                echo 'This is Post Build Stage'
            }            
        }
        stage('Java Version Check Stage') {
            steps {
                sh 'java --version'
            }            
        }
        
        stage('Success Stage') {
            steps {
                echo 'Successfully Build Thanks'
            }            
        }
    }
}
