// @Library('my-shared-library') _

pipeline {
    agent any
    options {
        skipDefaultCheckout true
    }
    stages {
        
        

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