pipeline {
    agent any

    parameters {
        string(defaultValue: "", description: 'get branch name', name: 'branchname')
    }

    stages {
        stage('PrintParameter'){
            steps{
                echo "You choose: ${params.branchname}"
            }
        }
    }
}
