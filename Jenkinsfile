// @Library('my-shared-library') _

pipeline {
    agent any
    stages {
        
        stage('Clean-up') {
            steps {
                cleanWs()
            }
        }

        stage('Build') {
            steps {
                // Get some code from a GitHub repository
                // git url: 'https://github.com/canerdikkollu/nodejs-helloworld.git', branch: 'main'

                sh "ls"

                sh "pwd"
            }
        }
    }
}