pipeline {
    agent any

    stages {

        

        stage('Build Docker Image') {
            steps {
                script {
                    sh 'docker build -t python-app .'
                }
            }
        }

        stage('Run Container') {
            steps {
                script {
                    sh 'docker run -d -p 5000:5000 python-app'
                }
            }
        }
    }
}
