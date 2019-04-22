node {
   stage('Check The sources files')
   {
      checkout scm
      }
   stage('Running the playbooks')
    {
        ansiblePlaybook(
            playbook: 'playbooks/webserver.yml',
            inventory: 'inventories/inventory.ini',
            credentialsId: 'ansible_jenkins')
         }
   stage('Delete workspace')
        {
           deleteDir()
        }
}
