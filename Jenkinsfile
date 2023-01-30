pipeline {
  agent any
  environment {
 ANSIBLE_PRIVATE_KEY=credentials(redis-ohio.pem)
 }
 
  stages {
    stage('SCM') {
      steps {
       
       sh 'ansible-playbook -i hosts --private-key=$ANSIBLE_PRIVATE_KEY playbook.yml'
      }
    }
  }
}
