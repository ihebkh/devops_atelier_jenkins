pipeline {
    agent any
    tools {
        maven 'M2_HOME'
    }
    stages {
        stage('GIT') {
            steps {
                git branch: 'master',
                    url: 'https://github.com/ihebkh/devops_atelier_jenkins.git'
            }
        }
    }
}
