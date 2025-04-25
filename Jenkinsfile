pipeline {
    agent any
    parameters{
        string(name: 'Branch_name', defaultValue: 'main', description: 'branch to work on')
       choice(name: 'ENV', choices: ['dev', 'staging', 'prod'], description: 'Select the environment')
    }
    

    stages {
        stage('good') {
            steps {
                echo 'Hi'
            }
        }
         stage('myguy') {
            steps {
                echo 'Howfar'
            }
        }
        stage('gitcheckout') {
            steps {
                checkout scmGit(branches: [[name: '*/feature-fisayo']], extensions: [], userRemoteConfigs: [[credentialsId: 'github credential  ', url: 'https://github.com/adenijifisayo/IBT-.git']])
                bat 'dir '
            }
        }
    }
}
