pipeline {
    agent any
    stages {
        stage("Compile") {
            steps {
                sh 'javac Test.java'
            }
        }

        stage("Run") {
            steps {
                sh 'java Test'
            }
        }
    }
}
