pipeline {
    agent any
    stages {
        stage('Clean') {
            steps {
                echo 'Cleaning...'
                bat 'mvn clean'
            }
        }
        stage('Package') {
            steps {
                echo 'Packaging...'
                bat 'mvn package'
            }
        }
        stage('Build') {
            steps {
                echo 'Building...'
                bat 'mvn install'
            }
        }
        stage('Test') {
            steps {
                echo 'Running tests...'
                bat 'mvn test'
            }
        }
    }
}
