pipeline {
    agent any

    stages {
        stage('Git') {
            steps {
                git branch: 'main', url: 'https://github.com/Kamalesh-Devi/docker.git'
            }
        }
        stage('build and run') {
            steps {
                sh '''docker build -t jimgg .
                    docker run jimgg'''
            }
        }
        
    }
}
