pipeline {
    agent {
        label 'ansible'
    }
    stages {
        stage('Build') {
            steps {
                sh "git clone 'https://github.com/Tourker/docker-molecule.git'"
            }
        }
        stage('Test role') {
            steps {
                sh "cd docker-molecule/simple/ && molecule test"
            }
        }
    }
}
