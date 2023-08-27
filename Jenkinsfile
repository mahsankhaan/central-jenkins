pipeline {
  agent any

    stages {

        stage('Code Checkout') {      
            steps {
 

              // get branch name
              
              //def branch = GIT_BRANCH


              println 'Getting current Branches'        
              println GIT_BRANCH
              //def branch = GIT_BRANCH
                checkout([
                    $class: 'GitSCM', 
                    //branches: [[name: '*/sandbox']], 
                    branches: [[name: GIT_BRANCH]], 
                    userRemoteConfigs: [[url: 'https://github.com/mahsankhaan/build-scalable-application-using-ibmcloud-docker.git']]
                ])
            }
        }

        stage(' Unit Testing') {
            steps {
                sh """
                echo "Running Unit Tes"
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
