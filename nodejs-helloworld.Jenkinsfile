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
                echo "denemeee"
                // sayHello "test"
                sh "git clone https://github.com/canerdikkollu/nodejs-helloworld.git"
            }
        }

    } 
}