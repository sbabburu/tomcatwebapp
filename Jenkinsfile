pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                bash 'mvn clean package'
                bash "docker build . -t tomcatwebapp:${env.BUILD_ID}"
            }
        }
    }
}
