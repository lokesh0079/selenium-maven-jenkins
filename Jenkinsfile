pipeline {
    agent any

    tools {
        maven 'MAVEN'
        jdk 'JDK'
    }

    stages {

        stage('Checkout') {
            steps {
                git 'https://github.com/lokesh0079/selenium-maven-jenkins.git'
            }
        }

        stage('Build') {
            steps {
                bat 'mvn clean install'
            }
        }

        stage('Test') {
            steps {
                bat 'mvn test'
            }
        }
    }
}
