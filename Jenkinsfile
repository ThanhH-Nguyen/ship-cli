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
                sh 'yarn global add bolt'
                sh 'bolt install'
                sh 'npm run dev:link'
                sh '/usr/local/bin/reactship --version'
            }
        }
    }
}
