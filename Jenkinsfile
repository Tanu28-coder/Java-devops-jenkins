pipeline {
    agent any

    tools {
        maven 'MAVEN3.9.12'
    }

    stages {

        stage('Checkout') {
            steps {
                git 'https://github.com/Tanu28-coder/Java-devops-jenkins.git'
            }
        }

        stage('Build') {
            steps {
                sh 'mvn clean package'
            }
        }

        stage('Build Docker Image') {
            steps {
                sh 'docker build -t java-devops-app .'
            }
        }

        stage('Run Docker Container') {
            steps {
                sh 'docker run -d --name java-container java-devops-app'
            }
        }
    }
}
