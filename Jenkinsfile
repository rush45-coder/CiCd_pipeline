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
    post{
        always{
            sh 'echo "always"'
        }
        success{
            sh 'echo "success"'
        }
        failure{
            sh 'echo "failure"'
        }
    }
}
