pipeline {
    agent {
        label 'master'
    }
    stages {
        stage('creating_venv') {
            steps {
                sh 'printenv'
                githubNotify description: 'This is a shorted example',  status: 'SUCCESS', repo: 'test_github_notification', credentialsId:'962985b3-2f06-4e6f-b534-3aab4c2fa9b2', account: 'flurin-conradin', sha: GIT_COMMIT  
            }
        }
    }
}
