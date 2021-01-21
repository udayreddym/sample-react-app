pipeline {
    agent {
        label 'docker'
    }
    // agent {
    //    docker {
    //         image "node:6-apline"
    //         args "-p 3000:3000"
    //    }
    // }
    stages {
        agent {
            docker {
                label 'docker'
                image "node:6-apline"
                args "-p 3000:3000"
            }
        }
        stage("Build") {
            steps {
                sh "npm install"
            }
        }
    }
}
