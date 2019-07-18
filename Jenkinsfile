pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'echo $(pwd)'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying'
            }
        }
    }
}