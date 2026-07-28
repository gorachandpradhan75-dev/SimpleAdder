pipeline {
    agent any

    tools {
        maven 'Maven-3.9.16'
    }

    stages {
        stage('Validate') {
            steps {
                bat 'mvn validate'
            }
        }

        stage('Compile') {
            steps {
                bat 'mvn compile'
            }
        }

        stage('Test') {
            steps {
                bat 'mvn test'
            }
        }

        stage('Package') {
            steps {
                bat 'mvn package'
            }
        }

        stage('Verify') {
            steps {
                bat 'mvn verify'
            }
        }

        stage('Install') {
            steps {
                bat 'mvn install'
            }
        }

        stage('Site') {
            steps {
                bat 'mvn site'
            }
        }

        stage('Clean') {
            steps {
                bat 'mvn clean'
            }
        }
    }
}