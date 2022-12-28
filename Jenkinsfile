pipeline 
{
    
  agent any
  
  parameters {
    string description: 'python script to exectute', name: 'script_name'
    }


  stages {
      
    stage("Git Checkout"){
            steps{
                git credentialsId: 'sahmed448', url: 'https://github.com/sahmed448/pipeline'
            }
        } 
      
    stage('version') {
      steps {
        sh 'python3 --version'
      }
    }
    
    stage('hello') {
      steps {
        sh 'python3 ${params.script_name}'
      }
    }
    
    
  }
}
