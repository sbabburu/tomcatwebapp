pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'package'
                sh "docker build . -t tomcatwebapp:${env.BUILD_ID}"
            }
        }
    }
}
