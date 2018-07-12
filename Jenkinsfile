pipeline {
    agent {
        label 'master'
    }
    stages {
        stage('creating_venv') {
            steps {
                sh 'printenv'
                githubNotify description: 'This is a shorted example',  status: 'SUCCESS', repo: 'test_github_notification', credentialsId:'flurin-private-github-notify', account: 'flurin-conradin', sha: GIT_COMMIT  
            }
        }
    }
}
