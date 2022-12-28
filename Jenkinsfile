pipeline 
{
    
  agent any
  
  parameters {
    string description: 'python script to exectute', name: 'script_name'
    }


  stages {
      
      
      
    stage('version') {
      steps {
        sh 'python3 --version'
      }
    }
    
    stage('hello') {
      steps {
        sh 'python3 $script_name'
      }
    }
    
    
  }
}
