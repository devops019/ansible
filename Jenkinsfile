pipeline{
    agent any
    stages{
        stage("installing apache"){
            steps{
                ansiblePlaybook credentialsId: 'awsSSH_key', inventory: 'hosts.inv', playbook: 'apache.yml'
            }
        }
    }
}