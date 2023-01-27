pipeline{
    agent any

    stages {

        stage ('Build Docker Image') {
            step {
                script {
                    dockerapp = docker.buildl("lheck/kube-news:${env.BUILD_ID}", '-f ./src/Dockerfile')
                } 
            } 
        }    
    }
}