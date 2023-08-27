pipeline {
    agent any

    parameters {
        string(defaultValue: "", description: 'K', name: 'HELLO')
    }

    stages {
        stage('PrintParameter'){
            steps{
                script{
                 sh 'echo ${params.HELLO}'
                }
            }
        }
    }
}
