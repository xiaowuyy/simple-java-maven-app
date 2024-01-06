pipeline {
    agent {
        docker {
            image 'maven:latest'
            args '-u 0:0 -v /root/.m2:/root/.m2 --net=host'
        }
    }
    stages {
        stage('Build') {
            steps {
                sh 'mvn -B -DskipTests clean package'
            }
        }
    }
}