pipeline {
    agent {
        label 'master'
    }
    parameters {
        booleanParam defaultValue: false , description: '', name: 'deploy_beta'
    }
    stages {
        stage('creating_venv') {
            steps {
                sh 'printenv'
                echo ${deploy_beta}
            }
        }
    }
}
