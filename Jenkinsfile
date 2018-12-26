pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'clean package'
                sh "docker build . -t tomcatwebapp:${env.BUILD_ID}"
            }
        }
    }
}
