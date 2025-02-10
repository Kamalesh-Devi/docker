pipeline {
    agent any

    stages {
        stage('Git-java') {
            steps {
              git branch: 'main', url: 'https://github.com/Kamalesh-Devi/docker.git'
            }
        }
         stage('Docker build and run') {
            steps {
              sh '''docker build -t myimg .
                    docker run myimg'''
            }
        }
        
    }
}
