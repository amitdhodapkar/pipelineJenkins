pipeline {
    agent any
    stages {
        stage('Activation_Test') {
            steps {
                echo 'Testing Activation code'
                publishHTML target: [
                        allowMissing: false,
                        alwaysLinkToLastBuild: false,
                        keepAll: true,
                        reportDir: 'reports',
                        reportFiles: 'index.html',
                        reportName: 'DSP Validation Report'
                      ]
                  }
        }
    }    
}
