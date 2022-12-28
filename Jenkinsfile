pipeline 
{
    
  agent any
    
  parameters {
     string(name: 'script_name', description: 'script name to execute')
    }

  stages {
             
      
    stage('version') {
      steps {
        sh 'python3 --version'
      }
    }
    
    stage('hello') {
      steps {
          sh 'python3  /var/jenkins_home/${params.script_name}'
      }
    }
    
    
  }
}
