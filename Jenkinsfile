

pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'mkdir -p out'
                sh 'javac -d out src/Main.java'
            }
        }

        stage('Run') {
            steps {
                sh 'java -cp out Main'
            }
        }
    }
}
