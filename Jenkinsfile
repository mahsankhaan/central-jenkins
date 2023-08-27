pipeline {
    agent any

    parameters {
        string(defaultValue: "", description: 'K', name: 'branchname')
    }

    stages {
        stage('PrintParameter'){
            steps{
                echo "You choose: ${params.branchname}"
            }
        }
    }
}
