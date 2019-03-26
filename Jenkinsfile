pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                sh 'docker build -t audi07/test:$BUILD_NUMBER -f Dockerfile .'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
               
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
                sh 'docker push audi07/test:$BUILD_NUMBER'
            }
        }
    }
}
