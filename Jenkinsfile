pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'docker run --rm -v /root/.m2:/root/.m2 -B maven:3.6.2-jdk-11-slim -DskipTests clean package'
            }
        }
    }
}