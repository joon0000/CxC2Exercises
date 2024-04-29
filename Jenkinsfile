pipeline {
    
    agent any  

    stages {
        stage('Check Permissions') {
            steps {
                sh 'pwd'
                sh 'ls -lha'
            }
        }
        stage('Checkmarx') {
            steps {
                echo 'Checkmarx'
                checkmarxASTScanner additionalOptions: '', baseAuthUrl: '', branchName: '', checkmarxInstallation: 'cx', credentialsId: '', projectName: 'CxE-pipe2', serverUrl: '', tenantName: '', useOwnAdditionalOptions: true
            }
        }

        stage('Test') {
            steps {
                sh 'pwd'
                sh 'ls -lha'
            }
        }
    }
}