pipeline {
    agent any
    stages {
        stage('Clone') {
            steps {
                git branch: 'dev', url: 'https://github.com/samirkariya/workshop.git'
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
