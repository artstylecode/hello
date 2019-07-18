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
        stage('Build images') {
            steps {
                sh 'mkdir -p /go/binary/'
                sh 'cp conf /go/binary/ -R'
                sh 'cp views /go/binary/ -R'
                sh 'cp hello /go/binary/ -R'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying'
            }
        }
    }
}