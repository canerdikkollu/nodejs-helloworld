@Library('my-shared-library') _

pipeline {
    agent any
    stages {
        
        environment {
            DOCKERHUB_CRED=credentials('docker-hub-credential')
        }

        stage('Set Environment') {
            steps {
                script {
                    APP_IMAGE_REGISTRY = "canerdikkollu"
                    APP_IMAGE_REPOSITORY = "nodejs-helloworld"
                }
            }
        }

        stage('Hello') {
            steps {
                sayHello "caner"
            }
        }

        stage('Build') {
            steps {
                dockerBuild "${APP_IMAGE_REGISTRY}", "${APP_IMAGE_REPOSITORY}"
            }
        }

        stage('Push') {
            steps {
                dockerPush "${APP_IMAGE_REGISTRY}", "${APP_IMAGE_REPOSITORY}"
            }
        }

    }
}