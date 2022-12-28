pipeline 
{
    
  agent any
  

  stages {
      
    stage('version') {
      steps {
        sh 'python3 --version'
      }
    }
    
    stage('hello') {
      steps {
        sh 'python3  /var/jenkins_home/script1.py'
      }
    }
    
    
  }
}
