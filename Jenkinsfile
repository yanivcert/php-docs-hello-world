pipeline {
    agent any
    stages {
        stage('Get Source') {
            steps {
                 git url: 'https://github.com/yanivcert/php-docs-hello-world.git'              
            }
        }
        stage('Publish to Azure') {
            steps {
                azureWebAppPublish appName: 'jenkins27402-php', azureCredentialsId: 'mySp', 
                publishType: 'file', resourceGroup: 'Jenkins'
            }
        }  
    } 
}
