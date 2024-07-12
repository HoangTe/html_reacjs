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
                // This step should not normally be used in your script. Consult the inline help for details.
                credentialsId: 'push dockerhub') {
                // some block
                }
                sh label: '', script: 'docker build -t hoangte/t3h-repository .'
                sh label: '', script: 'docker push hoangte/t3h-repository'}
            }
        }
    }
}