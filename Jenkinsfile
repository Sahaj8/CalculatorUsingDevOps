pipeline {
    // The “agent” section configures on which nodes the pipeline can be run. 
    // Specifying “agent any” means that Jenkins will run the job on any of the 
    // available nodes.
		agent any 
    stages {
        stage('Git Pull') {
            steps {
                // Make sure to add your own git url and credentialsId
				git url: 'https://github.com/Sahaj8/CalculatorUsingDevOps.git', branch: 'main'
            }
        }
        // stage('Maven Build') {
        //     steps {
        //         // Maven build, 'sh' specifies it is a shell command
        //         sh 'mvn clean install'
        //     }
        // }
        //  stage('Docker build') {
        //     steps{
        //         script {
        //             imageName=docker.build "sahajv/scientific_calc"
        //         }
        //     }
        // }
        // stage('Docker push img') {
        //     steps {
        //         script{
        //             docker.withRegistry('','docker_cred'){
        //             imageName.push()
        //             }
        //         }    
        //     }
        // }
        // stage('Ansible Deploy') {
        //     steps {
        //         //Ansible Deploy to remote server (managed host)
        //         // ansiblePlaybook colorized: true, disableHostKeyChecking: true, installation: 'Ansible', inventory: 'inventory', playbook: 'p2.yml'
        //         ansiblePlaybook becomeUser: null, colorized: true, disableHostKeyChecking: true, installation: 'Ansible', inventory: 'inventory', playbook: 'p2.yml', sudoUser: null
        //     }
        // }
    }
}
