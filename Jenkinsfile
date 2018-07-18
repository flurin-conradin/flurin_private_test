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
        when {
             expression { params.DEPLOY_BETA == true }
        }
        stage('deploy_to_beta') {
            steps {
                sh 'printenv'
                echo "deploying to beta"
            }
        }
    }

}
