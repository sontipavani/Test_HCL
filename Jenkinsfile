pipeline {
    agent any
    
     
    stages {
      stage('Start') {
           steps {
             
                git branch: 'master', url: 'https://github.com/sontipavani/Test_HCL.git'
             
          }
        }
        
     
        
         stage('Build') {
           steps {
             
                echo 'Build'

          }
        }
        
        
         
        
        
        
        stage('Ansible Deploy') {
             
            steps {
                 
             
               
               echo 'Ansible Deploy'

               
            
            }
        }
    }
}
