pipeline {
    agent {
        docker {
            image 'node:10.14.2' 
            args '-p 3000:3000' 
        }
    }
    stages {
        stage('Build') { 
            steps {
                sh 'yarn --version' 
            }
        }
    }
}
