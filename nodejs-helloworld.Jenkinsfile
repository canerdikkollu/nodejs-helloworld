// @Library('my-shared-library') _

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
                // sayHello "test"
                sh '''
                    echo "denemeee"
                    
                    git clone https://github.com/canerdikkollu/nodejs-helloworld.git
                
                '''
            }
        }

    } 
}