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
                    sh 'npm run test-jenkins'
                }
            }
        }
        stage('Deploy') {
                    steps {
                        nodejs(nodeJSInstallationName: 'recent node') {
                            sh 'echo deployed'
                            sh 'tar czf results.tar.gz ./test-results.xml    '
                        }
                    }
                }

    }
    post {
                success {
                    junit '*.xml'
                    archiveArtifacts artifacts: 'results.tar.gz', fingerprint: true
                }
            }
}
