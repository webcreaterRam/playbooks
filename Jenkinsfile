pipeline {
    agent any
    stages {
        stage('Clone Repository') {
            steps {
                git 'https://github.com/webcreaterRam/playbooks.git'
            }
        }
        stage('Run Ansible Playbook') {
            steps {
                sh '''
                ansible-playbook -i hosts site.yml
                '''
            }
        }
    }
}
