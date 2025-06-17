pipeline {
    environment{
        version = '1.1.2'
    }
    tools{
        maven'maven_3.99'
        git'git_1.0.0'
    }
    agent any

    stages {
        stage('Hello') {
            steps {
                echo 'Hello World'
                bat '''git clone https://github.com/adenijifisayo/IBT-.git '''
                 bat '''dir '''
                  bat '''mvn compile'''
                
            }
        }
    }
}
