pipeline {
    agent any
    tools {
        maven 'M2_HOME'  // Ensure that M2_HOME is correctly configured in Jenkins Global Tool Configuration
    }
    stages {
        stage('GIT') {
            steps {
                git branch: 'main',  // Ensure you use the correct branch name
                    url: 'https://github.com/ihebkh/devops_atelier_jenkins.git'
            }
        }
        stage('Build') {
            steps {
                sh 'mvn clean install'  // Runs Maven build commands
            }
        }
    }
}
