pipeline {
    agent any

    stages {
        stage('Prepare') {
            steps {
                git branch: 'main', url: 'https://github.com/GrayFix/mnt-8.4-elasticsearch-role.git/'
            }
        }
        stage('Run molecule') {
            steps {
                sh 'molecule test'
            }
        }
    }
}
