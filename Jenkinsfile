pipeline{
  agent any  
  stages{  
      stage("Run ansible playbook"){
        steps{
        ansiblePlaybook credentialsId: 'ssh-keygen', inventory: 'hosts', playbook: 'nginx_install.yaml', vaultTmpPath: ''
        
        }
      }
  }
}
