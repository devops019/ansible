pipeline{
    agent any
    stages{
        stage("installing apache"){
            steps{
                ansiblePlaybook credentialsId: 'awsSSH_key', disableHostKeyChecking: true, installation: 'Ansible', inventory: 'hosts.inv', playbook: 'apache.yml' 
            }
        }
    }
}