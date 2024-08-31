pipeline {
    agent any
    stages {
        stage('Clone Repository') {
            steps {
               git branch: 'master', url: 'https://github.com/sarikabharath/repo1.git' 
            }
        }
        stage('Build') {
            steps {
                sh 'mvn compile'
            }
        }
        stage('Test') {
            steps {
                sh 'mvn test'
            }
        }
        stage('Install') {
            steps {
                sh 'mvn clean install'
            }
        }
    }
