pipeline {
    agent any
    stages {
        stage('Build') { 
            steps {
                nodejs(nodeJSInstallationName: 'recent node') {
                    sh 'npm install' 
                }
            }
        }
        stage('Test') { 
            steps {
                nodejs(nodeJSInstallationName: 'recent node') {
                    sh 'npm test' 
                    sh 'pwd'
                }
            }
        }
    }
    post {
                success {
                    junit '*.xml'
                }
            }
}