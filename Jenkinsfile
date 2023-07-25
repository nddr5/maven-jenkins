pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                git 'https://github.com/nddr5/maven-jenkins/tree/main.git'
                sh 'mvn package'
            }
        }
        stage('Test') {
            steps {
                sh 'mvn test'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying...'
            }
        }
    }
}
