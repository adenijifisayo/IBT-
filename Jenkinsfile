pipeline {
    agent any

    parameters {
        string(name: 'Branch_name', defaultValue: 'main', description: 'Branch to work on')
        choice(name: 'ENV', choices: ['dev', 'staging', 'prod'], description: 'Select the environment')
    }

    stages {
        stage('gitcheckout') {
            steps {
                // Export the parameters as environment variables for Windows
                withEnv(["Branch_name=${params.Branch_name}", "ENV=${params.ENV}"]) {
                    bat '''
                        echo Branch selected: %Branch_name%
                        echo Environment selected: %ENV%
                        git clone -b %Branch_name% https://github.com/adenijifisayo/IBT-.git
                        dir
                    '''
                }
            }
        }
    }
}
