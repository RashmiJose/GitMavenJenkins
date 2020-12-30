pipeline {
    agent any

    stages {
        stage('Cloning') {
            steps {
                git 'https://github.com/RashmiJose/MavenGit.git'
            }
       }     
       stage('Clean') {
            steps {
                bat 'mvn clean'
            }   
       }
       stage('Install') {
            steps {
                bat 'mvn install'
            }   
       }
       stage('Version') {
            steps {
                bat 'mvn -v'
            }   
       }
    }
}
