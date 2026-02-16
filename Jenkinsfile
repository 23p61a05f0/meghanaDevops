pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                git branch: 'ece',
                    url: 'https://github.com/23p61a05f0/meghanaDevops.git',
                    credentialsId: 'github-token'
            }
        }

        stage('Build') {
            steps {
                sh 'javac sample.java'
            }
        }

        stage('Run') {
            steps {
                sh 'java sample'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying the job'
            }
        }
    }
}
