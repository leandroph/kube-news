pipeline{
    agent any

    stages {

        stage ('Build Docker Image') {
            step {
                script {
                    dockerapp = docker.buildl("lheck/kube-news:v1", '-f ./src/Dockerfile')
                } 
            } 
        }    
    }
}