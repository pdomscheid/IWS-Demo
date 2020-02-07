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
    }

    stages {
        steps {
                nodejs(nodeJSInstallationName: 'recent node') {
                    sh 'npm test' 
                }
            }
    }
}