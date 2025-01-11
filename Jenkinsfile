pipeline {
    agent { label 'slave01' }
    stages {
        stage('Grafana Installation') {
            steps {
                sh '''
                export ANSIBLE_HOST_KEY_CHECKING=False
                ansible-playbook -i /etc/ansible/hosts /home/sony/ansible/Ansible_repo_bkp/grafana-site.yaml -vv
                '''
            }
        }
    }
}
