pipeline{
    agent any
    stages{
        stage('Git Clone'){
            steps{
                git branch: 'main', url: 'https://github.com/eoyebami/ansible-cluster.git'
        }
            
    }
        stage('Launching Ansible Playbook to deploy pod to k8 cluster'){
            steps{
                sh 'ansible-playbook ansible_cluster_deployment.yaml'
            }
        }    
    }
}