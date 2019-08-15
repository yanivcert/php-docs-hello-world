pipeline {
    agent any
    stages {
        stage('Get Source') {
            steps {
                 git url: 'https://github.com/yanivcert/php-docs-hello-world.git'              
            }
        }
    }
    post {
        always {
            archiveArtifacts '*.php'
        }
    } 
}
