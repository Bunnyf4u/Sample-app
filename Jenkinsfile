pipeline {

agent any

stages {

stage('Deploy Green') {

steps {

sh 'ansible-playbook -i /opt/ansible/hosts /opt/ansible/deploy_green.yml'

}

}

stage('Switch Traffic') {

steps {

sh 'ansible-playbook -i /opt/ansible/hosts /opt/ansible/switch_green.yml'

}

}

}

}
