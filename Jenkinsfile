pipeline {
    agent any
    stages {
        stage('Clone') {
            steps {
                git branch: 'main', url: 'https://github.com/YOUR-USERNAME/my-java-repo.git'
            }
        }
        stage('Compile') {
            steps {
                bat 'javac Hello.java'
            }
        }
        stage('Run') {
            steps {
                bat 'java Hello'
            }
        }
    }
}
