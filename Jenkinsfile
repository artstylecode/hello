pipeline {
    agent {
         docker { image 'registry.cn-shanghai.aliyuncs.com/artcoding/beego:lts' }
    }
    stages {
        stage('Build') {
            steps {
                 sh 'go build'
                sh 'echo $(docker ps)'
            }
        }
        stage('Build images') {
            steps {
               sh 'echo $(ls `/usr/local/go/`)'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying'
            }
        }
    }
}