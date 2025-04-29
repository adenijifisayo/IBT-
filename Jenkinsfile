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
                    env.BRANCH_NAME=='main'
                }
            }
            steps {
                echo 'chill'
            }
        }
    }
}
