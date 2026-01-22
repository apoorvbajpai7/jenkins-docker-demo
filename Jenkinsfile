pipeline {
    agent any

    stages {
        stage('Build Docker Image') {
            steps {
                sh 'docker build -t jenkins-demo:1.0 .'
            }
        }

        stage('Run Container') {
            steps {
                sh 'docker run --rm jenkins-demo:1.0'
            }
        }
    }
}
