pipeline {
    agent any
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
