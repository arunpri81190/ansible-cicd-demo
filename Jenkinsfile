pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/arunpri81190/ansible-cicd-demo.git'
            }
        }
        stage('Run Ansible Playbook') {
            steps {
                sh 'ansible-playbook -i inventory.ini playbooks/deploy_time.yml'
            }
        }
    }
}
