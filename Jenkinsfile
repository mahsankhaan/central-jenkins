pipeline {
  agent any

    stages {

        stage('Code Checkout') {      
            steps {
 

              // get branch name
              def branch = GIT_BRANCH


              println 'Getting current Branchss'        
              println GIT_BRANCH

                checkout([
                    $class: 'GitSCM', 
                    branches: [[name: '*/sandbox']], 
                    userRemoteConfigs: [[url: 'https://github.com/mahsankhaan/build-scalable-application-using-ibmcloud-docker.git']]
                ])
            }
        }

        stage(' Unit Testing') {
            steps {
                sh """
                echo "Running Unit Tests"
                """
            }
        }

        stage('Code Analysis') {
            steps {
                sh """
                echo "Running Code Analysis"
                """
            }
        }

 

    }   
}
