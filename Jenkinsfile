pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'ls'
                sh '$ echo $PWD'
                sh 'docker run -v /root/.m2:/root/.m2 maven:3-alpine mvn -B -DskipTests clean package'
            }
        }
    }
}