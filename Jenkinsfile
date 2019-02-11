pipeline {
    agent any
    stages {
        stage('Release_Test') {
            steps {
                echo 'Testing Release code'
                  }
        }
        stage('Result_Test') {
            steps {
                publishHTML target: [
                        allowMissing: false,
                        alwaysLinkToLastBuild: false,
                        keepAll: true,
                        reportDir: 'reports',
                        reportFiles: 'index.html',
                        reportName: 'DSP Release Validation Report'
                      ]
                  }
            }
    }    
}
