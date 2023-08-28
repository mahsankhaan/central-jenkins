pipeline {
    agent any


    stages {
        stage('Start'){
            steps{
                script{
                //def branchname = "${params.PARAMETER01}"
                def branchname = GIT_BRANCH
                def branch = "test"


                echo branchname

            
                build job: 'input', wait: false, parameters: [string(name: 'branchname', value: branchname )]

                }
            }
        }
    }
}
