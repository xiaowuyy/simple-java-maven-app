pipeline {
    agent {
        docker {
            image 'maven:latest'
            args '-v /root/.m2:/root/.m2'
        }
    }
    stages {
        stage('Build') {
            steps {
                sh 'while true; do sleep 10;done'
            }
        }
    }
}