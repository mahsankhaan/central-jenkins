pipeline {
    agent any

    parameters {
        string(defaultValue: "", description: 'K', name: 'HELLO')
    }

    stages {
        stage('PrintParameter'){
            steps{
                echo "You choose: ${params.HELLO}"
            }
        }
    }
}
