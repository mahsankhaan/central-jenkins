pipeline {
    agent any
    stages {
        stage('Start'){
            steps{
                script{

                def branchname = "testme"
            
                build job: 'input', wait: false, parameters: [string(name: 'branchname', value: branchname )]

                }
            }
        }
    }
}
