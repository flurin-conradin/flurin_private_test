pipeline {
    agent {
        label 'master'
    }
    stages {
        stage('creating_venv') {
            steps {
                sh 'printenv'
                githubNotify description: 'This is a shorted example',  status: 'SUCCESS', repo: 'test_github_notification', credentialsId:'351186c5-1e9f-45db-be63-4f1507c92307', account: 'flurin-conradin', sha: GIT_COMMIT  
            }
        }
    }
}
