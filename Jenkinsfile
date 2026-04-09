pipeline {
    agent any


    stages {
        stage("Clone Repo") {
            steps {
                git branch: 'master', url: 'https://github.com/kadimasum/java-todo.git'
            }
        }

        stage("Prepare") {
            steps {
                sh 'chmod +x gradlew'
            }
        }

        stage("Build") {
            steps {
                sh './gradlew build'
            }
        }

        stage("Test") {
            steps {
    
    stages{
        stage("Clone repo"){
            steps{
                git branch:'master', url: 'https://github.com/kadimasum/java-todo.git'
            }
        }
        
        stage("Build code"){
            steps{
                sh './gradlew build'
            }
        }
        
        stage("Test code"){
            steps{
                sh './gradlew test'
            }
        }
    }
}
