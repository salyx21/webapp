pipeline {
    agent {
        label 'main-host'
    }

    stages {
        stage('Build') {
            steps {
                sh "docker build -t webapp:${BUILD_NUMBER} ."
            }
        }
        stage('Push to Dockerhub') {
            steps {
                echo 'psuh '
            }
        }
        stage('Deploy') {
            steps {
                sh 'deploy'
            }
        }
    }
}