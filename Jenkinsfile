pipeline {
    agent any
    stages {
        stage('Build') { 
            steps {
                sh 'apk add --update nodejs nodejs-npm'
                sh 'apk add yarn'
                sh 'yarn global add bolt'
                sh 'bolt install'
                sh 'npm run dev:link'
                sh '/usr/local/bin/reactship --version'
            }
        }
    }
}
