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
                    
                }
            }
            post {
                success {
                    junit './test-results.xml'
                }
            }
        }
    }
}