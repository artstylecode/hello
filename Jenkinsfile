pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo $(pwd)
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