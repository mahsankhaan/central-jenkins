pipeline {
    agent any

    parameters {
        string(defaultValue: "123", description: 'This is a parameter', name: 'PARAMETER01')
    }

    stages {
        stage('Start'){
            steps{
                script{
                echo "You choose: ${params.PARAMETER01}"

                def branchname = "${params.PARAMETER01}"
            
                build job: 'input', wait: false, parameters: [string(name: 'branchname', value: branchname )]

                }
            }
        }
    }
}
