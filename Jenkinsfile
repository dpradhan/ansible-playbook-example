pipeline {
    agent {
        node {
            label 'task01'
        }
    }
    stages {
        stage ('Create Environment') {
            steps {
                //call Ansible Tower playbook deploy here.    
            }
        }
        stage ('Deploy Cluster') {
            steps {
                //call Ansible Tower or kubectl to deploy kub cluster
            }
        }
        stage ('Execute tests') {
            steps {
                // exeute test inside a docker container
            }    
        }
        stage ('Delete Cluster') {
            steps {
                // call ansible Tower or kubectl to remove kub cluster
            }
        }
        stage ('Delete Env') {
            steps {
                //Call Ansible Tower to execute playbook to
                //remove AKS
                //remove Dbaas
            }
        }
    }
}