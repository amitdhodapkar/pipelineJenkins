pipeline {
    agent any
    stages {
        stage('Dev_Test') {
            steps {
                echo 'Testing Dev code'
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
                        reportName: 'DSP Dev Validation Report'
                      ]
                  }
            }
    }    
}
