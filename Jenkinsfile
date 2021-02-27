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
             
                sh 'mvn package'

          }
        }
        
        
         
        
        
        
        stage('Ansible Deploy') {
             
            steps {
                 
             
               
               sh "ansible-playbook main.yml -i inventories/dev/hosts --user jenkins --key-file ~/.ssh/id_rsa"

               
            
            }
        }
    }
}
