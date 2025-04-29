pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                echo 'Hello World'
            }
        }
        stage('damnbro') {
            when{
                expression{
                    BRANCH_NAME=='main'
                }
            }
            steps {
                echo 'chill'
            }
        }
    }
}
