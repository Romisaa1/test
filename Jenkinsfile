pipeline {
    agent any

    parameters {
        string(name: 'USERNAME', description: 'Enter your name')
        choice(name: 'ENVIRONMENT', choices: ['dev', 'test', 'prod'], description: 'Select environment')
        booleanParam(name: 'DEPLOY', description: 'Deploy after build?')
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
