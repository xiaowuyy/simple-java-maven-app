pipeline {
    agent {
        docker {
            image 'maven:paas'
            args ' -v /root/.m2:/root/.m2 --net=host'
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