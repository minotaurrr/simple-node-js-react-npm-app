pipeline {
    agent {
        docker {
            image 'node:6-alpine' 
            args '-p 3000:3000' 
        }
    }
    environment {
        HTTP_PROXY = 'http://n102518:Bhk2012@http-gw.tcif.telstra.com.au:8080'
        HTTPS_PROXY = 'http://n102518:Bhk2012@http-gw.tcif.telstra.com.au:8080'
    }
    stages {
        stage('Build') { 
            steps {
                sh 'npm install' 
            }
        }
    }
}
