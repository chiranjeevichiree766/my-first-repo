pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                script {
                    docker.build('my-app')
                }
            }
        }
        stage('Run') {
            steps {
                script {
                    docker.image('my-app').run('-d -p 8080:8080')
                }
            }
        }
    }
}
