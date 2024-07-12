pipeline {
    agent any
    stages{
        stage('Clone') {
            steps {
                git branch: 'main', credentialsId: 'github', url: 'https://github.com/HoangTe/html_reacjs.git'
            }
        }
        stage('Push Docker Hub') {
            steps {
                git branch: '', credentialsId: 'push dockerhub', url: ''
                // some block
                sh label: '', script: 'docker build -t hoangte/t3h-repository:2.0 .'
                sh label: '', script: 'docker push hoangte/t3h-repository:2.0'}
            }
        }
    }
}