pipeline {
    agent any
    
    tools{
        maven "Maven-3.9.10"
    }    

    stages {
        
        stage('Docker Pull Image push'){
             steps{
                   sh 'docker pull ananderic/ecomm_backend_api'
            }
        }
        stage('kubernetes deployment'){
            steps{
             sh 'kubectl apply -f Deployment.yml'
            }
        }        
    }
}
