pipeline {
    agent any


    stages {
        stage('run script') {
            steps {
                sh 'chmod +x ./test.sh'
                sh './test.sh'

            }
        }
    }
}
