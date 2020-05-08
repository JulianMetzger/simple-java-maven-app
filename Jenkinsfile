pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'docker run --rm -v /root/.m2:/root/.m2 maven:3.6.2-jdk-11-slim -B -DskipTests clean package'
            }
        }
    }
}