pipeline {
    
    agent any  

    stages {
        stage('Check Permissions') {
            steps {
                sh 'pwd'
                sh 'chmod -R 777 /var/jenkins_home/workspace/CxE-pipe2'
            }
        }
        // stage('Checkmarx') {
        //     steps {
        //         echo 'Checkmarx'
        //         checkmarxASTScanner additionalOptions: '--project-groups My-POC-Group --scan-types sast --report-format pdf', baseAuthUrl: '', branchName: '', checkmarxInstallation: 'cx', credentialsId: '', projectName: 'jenkins-pipeline', serverUrl: '', tenantName: '', tenantName: '', useOwnAdditionalOptions: true
        //     }
        // }

        // stage('Test') {
        //     steps {
        //         sh 'pwd'
        //         sh 'ls -lha'
        //     }
        // }
    }
}