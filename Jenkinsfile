node {
   deleteDir()
   checkout scm
  
        ansiblePlaybook(
            playbook: 'ping.yml',
            inventory: 'inventory.ini',
            credentialsId: 'ansible_jenkins')
}
