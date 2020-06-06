pipeline {
    agent any
    stages {
        stage('Prep') {
            steps {
                echo 'Running build automation - prep'
            }
        }
        stage('validate') {
            steps {
                echo 'Running build automation - validate'
            }
        }    
        stage('Ansible') {
            steps {
                echo 'Running build automation - ansible'
                ansiblePlaybook(playbook: 'create_dir.yml')
            }
        }    
    }
}
