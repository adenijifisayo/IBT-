pipeline {
    agent any

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
