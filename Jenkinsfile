node {
    stage ('git clone'){
        git 'https://github.com/kesavapandiyan/clearwater-heat.git'
    }
    
    
    
    stage ('Approve'){
            input 'review git and approve'
               
           }
    stage ('run playbook'){
            sh 'ansible all -m ping --sudo -u root'
            sh 'ansible-playbook -v ansible_playbook.yaml --sudo -u root'
    }
}
