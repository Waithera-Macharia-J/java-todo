pipeline {
    agent any
    stages{
        stage('Clone REpo'){
            steps{
                git branch: 'master', url: 'https://github.com/Waithera-Macharia-J/java-todo.git'
            }
        }
        stage ('Build Repo'){
            steps{
                sh './gradlew clean build'
            }
        }
        stage ('Test Cpde'){
            steps{
                sh './gradlew test'
            }
        }
    }
}