pipeline {
    agent any


    stages {
        stage('Start'){
            steps{
                script{
                def branchname = GIT_BRANCH
                when {
                branch 'main'
                 }
                build job: 'input', wait: false, parameters: [string(name: 'branchname', value: branchname )]

                }
            }
        }
    }
}
