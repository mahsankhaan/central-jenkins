pipeline {
    agent any


    stages {
        stage('Start'){
            steps{
                script{
                def test = "this"
                def branchname = GIT_BRANCH
                build job: 'input', wait: false, parameters: [string(name: 'branchname', value: branchname )]

                }
            }
        }
    }
}
