@Library('my-shared-library') _

pipeline {
    agent any

    stages {
        stage('Clean-up') {
            steps {
                cleanWs()
            }
        }

        stage('Cloning Repositories') {
            steps {
                script {
                    ls
                    pwd
                }
            }
        }

    } 
}