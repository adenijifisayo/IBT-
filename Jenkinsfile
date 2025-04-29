pipeline {
    environment{ 
        version = '1.2.2'
    }
    agent any

    stages {
        stage('Hello') {
            steps {
                echo 'Hello World'
                echo '{env.version}'
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
