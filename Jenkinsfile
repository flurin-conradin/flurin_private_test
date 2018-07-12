pipeline {
    agent {
        label 'master'
    }
    stages {
        stage('creating_venv') {
            steps {
                sh 'printenv'
                githubNotify description: 'This is a shorted example',  status: 'SUCCESS', repo: 'TL_ASR_DataCollection', credentialsId:'flurin-telepathy-github-key', account: 'flurin-telepathy-ai', sha: GIT_COMMIT  
            }
        }
    }
}
