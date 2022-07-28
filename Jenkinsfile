pipeline {
    agent {
        docker {
            image 'node:6-alpine' 
            args '-p 8081:8081' 
        }
    }
    stages {
        stage('Build') { 
            steps {
                sh 'npm install' 
            }
        }
    }
}
