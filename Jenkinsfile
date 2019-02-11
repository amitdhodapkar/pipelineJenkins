pipeline {
    agent any
    stages {
        stage('Iteration_Test') {
            steps {
                echo 'Testing Iteration code'
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
                        reportName: 'DSP Activation Validation Report'
                      ]
                  }
            }
    }    
}
