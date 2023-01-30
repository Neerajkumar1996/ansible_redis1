pipeline {
  agent any
 
  stages {
    stage('SCM') {
      steps {
       
        sh 'ansible-playbook -i hosts --private-key=private-key playbook.yml'
      }
    }
  }
}
