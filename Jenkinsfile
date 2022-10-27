pipeline {
    agent { label 'NODE' }
    stages {
        stage('vcs') {
            steps {
                git url: 'https://github.com/Nagaraju11111/python-webcount.git',
                    branch: 'master'
            }
        }
        stage('build') {
            steps {
                sh 'pip3 install -r requirements.txt'
                sh 'tox'
            }
        }
    }
}
