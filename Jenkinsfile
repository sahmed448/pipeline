pipeline 
{
    
  agent any
    
  parameters {
     string(name: 'script_name', description: 'script name to execute')
    }

  stages {
             

    stage("Git Checkout"){
        steps{
                git branch: 'main', credentialsId: 'sahmed448-github-token', url: 'https://github.com/sahmed448/pipeline'
            }
        } 
      
    stage('version') {
      steps {
        sh 'python3 --version'
      }
    }
    
    stage('hello') {
      steps {
        sh 'python3  /var/jenkins_home/$params.script_name'
      }
    }
    
    
  }
}
