pipeline {
  agent any
 
  stages {
    stage('SCM') {
      steps {
       
        sh 'ansible-playbook -i hosts playbook.yml'
      }
    }
  }
}
