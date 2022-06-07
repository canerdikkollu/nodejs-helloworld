@Library('my-shared-library') _

pipeline {
    agent any
    stages {
        stage('Initialize'){
            def dockerHome = tool 'myDocker'
            env.PATH = "${dockerHome}/bin:${env.PATH}"
        }

        stage('Set Environment') {
            steps {
                script {
                    APP_IMAGE_REGISTRY = "canerdikkollu"
                    APP_IMAGE_REPOSITORY = "nodejs-helloworld"
                }
            }
        }

        stage('Build') {
            steps {
                sh "ls"

                sh "pwd"

                sayHello "caner"

                dockerBuild "${APP_IMAGE_REGISTRY}", "${APP_IMAGE_REPOSITORY}"
            }
        }

    }
}