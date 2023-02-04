pipeline {
    agent any

    stages {
        stage('scm') {
            steps {
                git branch: 'main', url: 'https://github.com/Neerajkumar1996/ansible_redis1.git'
            }
        }
    
           stage('check out') {
            steps {
         ansiblePlaybook credentialsId: 'ubuntu', disableHostKeyChecking: true, installation: 'ansible2', inventory: 'hosts', playbook: 'playbook.yml'
       
            }
        }
        
        
    }
}
