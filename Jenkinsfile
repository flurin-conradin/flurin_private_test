pipeline {
    agent {
        label 'master'
    }
    parameters {
        booleanParam defaultValue: false , description: '', name: 'DEPLOY_BETA'
    }
    stages {
        stage('creating_venv') {
            steps {
                sh 'printenv'
                echo "${DEPLOY_BETA}"
            }
        }
        stage('deploy_to_beta') {
            when {
                expression { params.DEPLOY_BETA == true }
            }
            steps {
                sh 'printenv'
                echo "deploying to beta"
            }
        }
    }

}
