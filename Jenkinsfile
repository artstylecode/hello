pipeline {
    agent {
         docker { image 'registry.cn-shanghai.aliyuncs.com/artcoding/beego:lts' }
    }
    stages {
        stage('Build') {
            steps {
                // sh 'go build'
                sh 'echo $(docker ps)'
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