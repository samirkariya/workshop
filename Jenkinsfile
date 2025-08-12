pipeline {
    agent any
    stages {
        stage('Clone') {
            steps {
                git branch: 'dev', url: 'https://github.com/YOUR-USERNAME/my-java-repo.git'
            }
        }
        stage('Compile') {
            steps {
                bat 'javac Loop.java'
            }
        }
        stage('Run in Dev Mode') {
            steps {
                bat 'java Loop'
            }
        }
    }
}
