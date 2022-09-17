pipeline {
    agent any
    stages {
        stage ("Get git") {
            steps {
                git "https://github.com/Andrey-Medvedtsev/example-playbook.git"
                
            }
        }
        stage(" execute Ansible") {
           steps {
                ansiblePlaybook installation: 'ansible', playbook: 'site.yml'
            }    
        }    
    }
}
