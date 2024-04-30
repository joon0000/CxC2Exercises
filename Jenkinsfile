pipeline {
    
    agent any  

    stages {
        stage('Check Permissions') {
            steps {
                sh 'pwd'
                sh 'ls -al'
                sh 'chmod -R 777 /var/jenkins_home/workspace/CxE-pipe2'
            }
        }
        stage('Checkmarx') {
            steps {
                echo 'Checkmarx'
                checkmarxASTScanner additionalOptions: '--project-groups My-POC-Group --scan-types sast', baseAuthUrl: '', branchName: '', checkmarxInstallation: 'cx', credentialsId: '', projectName: 'jenkins-pipeline', serverUrl: '', tenantName: '', useOwnAdditionalOptions: true
            }
        }

    }
}