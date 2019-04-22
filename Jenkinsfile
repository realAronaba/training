node {
   stage('Check The sources files')
   {
      checkout scm
      }
   stage('Running the playbooks')
    {
        ansiblePlaybook(
            playbook: 'uninstall_apache.yml',
            inventory: 'inventory.ini',
            credentialsId: 'ansible_jenkins')
         }
   stage('Delete workspace')
        {
           deleteDir()
        }
}
