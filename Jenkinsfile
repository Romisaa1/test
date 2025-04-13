pipeline {
    agent any

    parameters {
        string(name: 'USERNAME', defaultValue: 'romisaa', description: 'Enter your name')
        choice(name: 'ENVIRONMENT', choices: ['dev', 'test', 'prod'], description: 'Select environment')
        booleanParam(name: 'DEPLOY', defaultValue: true, description: 'Deploy after build?')
    }

    stages {
        stage('Print Params') {
            steps {
                echo "Hello, ${params.USERNAME}!"
                echo "Selected environment: ${params.ENVIRONMENT}"
                echo "Should deploy? ${params.DEPLOY}"
            }
        }
    }
}
