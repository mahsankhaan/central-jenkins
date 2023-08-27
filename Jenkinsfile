pipeline {
    agent any

    parameters {
        string(defaultValue: "123", description: 'This is a parameter', name: 'PARAMETER01')
    }

    stages {
        stage('Start'){
            steps{
                echo "You choose: ${params.PARAMETER01}"
                   
                


                script
                {
                    def branchvalue = ${params.PARAMETER01}
                }

                    build job: 'input', wait: false, parameters: [string(name: 'HELLO', value: 'branchvalue' )]
            }
        }
    }
}
