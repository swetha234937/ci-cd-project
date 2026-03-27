pipeline {
    agent any

    stages {
        stage('Build Docker Image') {
            steps {
                sh 'docker build -t swetha123/food-app:latest .'
            }
        }

        stage('Push Docker Image') {
            steps {
                sh 'docker login -u swetha123 -p swetha@1234'
                sh 'docker push swetha123/food-app:latest'
            }
        }
    }
}
