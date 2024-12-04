pipeline {
    agent {
        docker {
            image 'node:14'
            args '-v /var/run/docker.sock:/var/run/docker.sock'
        }
    }

    stages {
        stage('Build') {
            steps {
                echo 'Hello, World from a Docker container!'
                sh 'node --version'
            }
        }
    }
}
