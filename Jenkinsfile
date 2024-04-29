pipeline {
    
    agent any  

    stages {
        stage('Check Permissions') {
            steps {
                sh 'pwd'
                sh 'sudo chmod -R 777 /var/jenkins_home/workspace/CxE-pipe2'
                sh 'cd ..'
                sh 'pwd'
                sh 'ls -al | grep CxE-pipe2'
            }
        }
        // stage('Checkmarx') {
        //     steps {
        //         echo 'Checkmarx'
        //         checkmarxASTScanner additionalOptions: '', baseAuthUrl: '', branchName: '', checkmarxInstallation: 'cx', credentialsId: '', projectName: 'CxE-pipe2', serverUrl: '', tenantName: '', useOwnAdditionalOptions: true
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